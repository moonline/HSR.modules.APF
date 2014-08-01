====================================================
Zusammenfassung mit wichtigen Themen für die Prüfung
====================================================


Patterns
========

Singleton
---------

Mögliche Alternativen, um einen Singleton abzulösen:

* Zugriff auf andere Komponenten der Applikation wird benötigt -> Context Objekt injecten
* Anzahl Instanzen muss kontrolliert werden -> CRTP Limit object count for a class
* Jeder muss Zugang zu einem Objekt habe, z.B. Settings. -> Als Objekt der Applikation anhängen, über Kontext darauf zugreifen, nach Möglichkeit Read-Only
* Monostate: Klasse mir nur static Member -> Keine oder beliebig viele Instanzen, spielt aber keine Rolle, State ist global
* Instanzkontrolle: Ist eigentlich eine Aufgabe der Applikation und nicht eines Typs


Iterator
--------

* Hohe Bindung zwischen Iterator und Collection
* Niedrige Bindung zwischen Iterator und Verwendung

.. code-block:: java

	ArrayList<String> alist = new ArrayList<String>();
	// . . . Add Strings to alist

	for (Iterator<String> it = alist.iterator(); it.hasNext(); ) {
		String s = it.next();
	}
	
	
	/**
	 * Iterator
	 */
	public class MyIterator <T> implements Iterator<T> {
		private int position = 0;
		private MyCollection<T>;
		
		public void Iterator(MyCollection<T> col) { this.Collection = col; }
		
		public bool hasNext() {
			return this.collection.size() > this.position+1;
		}
		
		public T next() {
			this.position++;
			return this.collection.get(this.position);
		}
	}
	
	/**
	 * Collection
	 */
	 public class MyCollection<E> implements Iterable<E>{
		public Iterator<E> iterator() {
			return new MyIterator<E>(this);
		}
	}


Pattern Anwendung
=================

Pattern Combinations
--------------------

Häufig anzutreffende Pattern Kombinationen:

* Visitor und Composite (Visitors traversiert Composite-Struktur)
* Flyweight und Composite
* Strategy und NullObject (Defaultstrategy)
* Iterator und NullObject (Default Verhalten für Collections)
* Memento und Command (Undo)
* Template Method und Strategy (Flexibilisierung der Template Method)
* Prototype und Factory Method (Factory erstellt Objekte anhand von Bestehenden -> Prototype)


Frameworks
==========

Unterschied zwischen Library & Framework
----------------------------------------

Library
	wird von Applikation aufgerufen
FW
	* ruft Applikationscode auf (Don't call us, we call you)
	* Inversion of Control
	* Ist ein Programmskelett
	
	
Values
======

ValueObject oder String?
------------------------

Soll eine ISBN Nummer ein eigener Datentyp sein oder String? Wenn interner Aufbau unwichtg:
String, wenn Aufbau, Validation und Korrektheit wichtig: ISBN-Type


ValueObject
-----------

hashCode(), equals und ev. Serializable implementieren

.. code-block:: java

	public class ISBN {
		private String isbn;
		
		private static bool isValidISBN(String isbn) {
			return ...
		}
		
		public void ISBN(String isbn) {
			if(ISBN::isValidISBN(isbn) {
				this.isbn = isbn;
			} else {
				this.isbn = null;
			}
		}
		
		public String getISBN() { return new String(this.isbn); }
		
		public boolean equals(Object rhs) {
			return rhs instanceof ISBN && equals((ISBN) rhs;
		}
		
		public boolean equals(ISBN isbn) {
			return this.isbn.equals(isbn.getISBN());
		}
		
		public int hashCode() {
			return ...
		}
		
		// if needed: implement Serializable
	}
	

