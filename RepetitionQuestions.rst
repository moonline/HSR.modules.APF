==========================
FS14 APF Repetitionsfragen
==========================


Antworten zu den Repetitionsfragen
==================================
Falls vorhanden befinden sich diese im GitHub Repository. Ergänzungen oder ganze Antwortensets sind jederzeit herzlich willkommen. https://github.com/moonline/HSR.modules.APF



Symbolerklärung
===============
**[DP]**
Wissensfragen des Dozenten (Slides) für die Prüfung

**[EW]**
Wissensfrage, die über den Stoff der Vorlesung hinaus geht.



1 Patterns Allgemein
====================

**1.0.1.**
Was sind Patterns? Was zeichnen sie aus?

**1.0.2.**
Welche Inhalte beinhaltet eine gute Pattern Beschreibung?

**1.0.3.**
Warum sind KIS, DRY, SOLID, ... keine Patterns? Was grenzt sie von Patterns ab? Nennen sie zudem zwei Arten von Pattern-Ähnlichen Beschreibungen, die keine Patterns sind.

**1.0.4.**
Welche Arten von Patterns gibt es?

**1.0.5.**
Kommentieren Sie den Satz: "No Pattern is an Island".


2 Patterns
==========

**2.0.1.**
Erklären Sie die folgenden Patterns. Nennen Sie zu jedem
	i) Problemstellung
	ii) Lösung
	iii) Vor- / Nachteile
	iv) Verwandtschaften zu ähnlichen Patterns / Abgrenzung
	v) Einsatzbeispiele
	
a) Flyweight
b) Memento
c) Mediator
d) Visitor
e) Command
f) Iterator
g) Enumeration Method
h) Batch Method
i) State Pattern
	1) Object for States
	2) Methods for State
	3) Collections for States
	

3 Frameworks
============

**3.0.1.**
Was bringen Frameworks? Warum werden sie entwickelt und warum sollte man sie einsetzen?

**3.0.2.**
Was ist ein Framework überhaupt?

**3.0.3.**
Was ist ein Application Framework?

**3.0.4.**
Wie unterscheidet sich Framework und Bibliothekt? Skizzieren Sie den Aufruf, bzw. woher ihre Klasse die Schnittstelle hat.

**3.0.5.**
Wie funktionieren Framework Callbacks? Was ist das Konzept dahinter?

**3.0.6.**
Was sind Hooks? Was erlaubt ihnen das Framework damit?

**3.0.7.**
Was sind Micro-Frameworks?

**3.0.8.**
Warum sind die Patterns "Template Method", "Strategy", "Command Processor" und "Decoration" "Micro Frameworks"?


4 ValueObject
=============

**4.0.1.**
Was sind Values?

**4.0.2.**
Wo ist der Unterschied zwischen Value und Object?

**4.0.3.**
Michael Jackson definiert "Events", "Entities" und "Values". Erklären Sie die Begriffe und nennen Sie Beispiele.

**4.0.4.**
Kevlin Henney definiert "Entities", "Services", "Values" und "Tasks" als Objektkategorien. Erklären Sie die Begriffe und nennen Sie Beispiele.

**4.0.5.**
Erklären Sie die Objektcharakteristik "identity", "state" und "behaviour".

**4.0.6.**
Was sind Value Objects?

**4.0.7.**
Ein Buch (Author, Title, ISBN) besitzt eine ISBN Nummer. In welchem Fall ist es sinnvoller, die ISBN Nummer als String abzulegen und in welchem Fall ist es sinnvoller, dafür einen eigenen Typ zu definieren?

**4.0.8.**
In welchem Fall macht der Einsatz von Value Types in OO Sprachen Sinn?

**4.0.9.**
Welches Verhalten sollten Values bei equality ( .equals(..) ) aufweisen im Unterschied zu Objekten?

**4.0.10.**
Warum macht es bei Values keinen Unterschied, ob sie kopiert oder per Referenz übergeben werden?

**4.0.11.**
Welchen Vorteil bieten Values, was die Persistence angeht?

**4.0.12.**
Erklären Sie die Value Patterns:

.. image:: img/5.4.jpg


**4.0.13.**
Welches Problem löst "Whole Value"?

**4.0.14.**
Was ist ein "Value Object"? Wann wird es gebraucht? Wie wird in Java und C++ ein "Value Object" implementiert?

**4.0.15.**
Erklären Sie "Class Factory Method". Wozu dient das Pattern?

**4.0.16.**
Wie kann in einer Sprache die auf "Call by Reference" basiert, "Copied Value" umgesetzt werden? Wie kann allgemein verhindert werden, das ein übergebenes Objekt verändert wird? Machen Sie Beispiele für C++ und Java.

**4.0.17.**
Erklären Sie den Unterschied zwischen "Cloning" und "Prototype".

**4.0.18.**
Welche Idee verbirgt sich hinter dem Kopierkonstruktor?

**4.0.19.**
Was sind "Immutable Values" und "Immutable Companion"?

**4.0.20.**
Was ist "Mutable Companion"?


5 Reflection
============

**5.0.1.**
Was ist Reflection?

**5.0.2.**
Welche Probleme löst Reflection?

**5.0.3.**
Was sind Metaobjects?

**5.0.4.**
Skizzieren Sie das Reflection Pattern.

**5.0.5.**
Was sind Introspection und Intercession? Warum bieten viele Sprachen nur Introspection?

**5.0.6.**
Nennen Sie einige Sprachfeatures wie z.B. Polymorphism, die auf Reflection oder Reflection ähnliche Prozesse setzen.

**5.0.7.**
Wo werden Reflectionmechanismen eingesetzt? Machen Sie ein Paar Beispiele.

**5.0.8.**
Erklären Sie die folgenden Patterns. Nennen Sie auch, wie es konkret umgesetzt wird, Anwendungsgebiet und Vor- und Nachteile:

a) Type Object
b) Property List
c) Anything
d) Extension Interface

**5.0.8.**
Wie sinnvoll ist Reflection auf Reflection? Welche Probleme gibt es?

**5.0.9.**
Welche Nachteile besitzt Reflection?

**5.0.10.**
Welche Gefahren birgt Reflection?


6 Frameworkers Dilemma
======================

**6.0.1.**
Welche Vorteile bieten Application Frameworks und welche Probleme bringen sie mit sich?

**6.0.2.**
Wie werden Frameworks verwendet? Warum ist dies ein Kopplungsproblem?

**6.0.3.**
Welche Konsequenzen hat die starke Koppelung des eigenen Codes an das Framework und die Kopplung innerhalb des Frameworks?

**6.0.4.**
Warum können sich Frameworks nur langsam weiterentwickeln?

**6.0.5.**
Welche Wege gibt es, dieses Dilemma zu mindern?

**6.0.6.**
Nennen Sie 5 Technische Lösungen, die helfen das Dilemma zu minimieren.

**6.0.7.**
Was ist das "Encapsulate Context" Pattern? Wie funktioniert es?

**6.0.8.**
Was bringen "Property Lists" in diesem Zusammenhang?

**6.0.9.**
Wie funktioniert das Extension Interface Pattern? Erklären Sie, wie das IAdaptable in Eclipse funktioniert.



7 WAM
=====

**7.0.1.**
Was ist WAM? Was bedeutet es und wozu wird es benutzt?

**7.0.2.**
Was sind Knowledge Worker?

**7.0.3.**
Welches Leitbild steckt hinter WAM?

**7.0.4.**
Erklären Sie die folgenden Begriffe bezüglich WAM und das Konzept, das damit umgesetzt wird.

a) Material
b) Werkzeug
c) Arbeitsumgebung
d) Automat
e) Container

**7.0.5.**
Wie interagieren die folgenden Elemente (miteinander)?

a) Werkzeug und Material
b) Werkzeugentwurf
c) Materialentwurf

**7.0.6.**
Nennen Sie die Trade-offs und Design Charakeristiken von Werkzeugen.

**7.0.7.**
Was stellt die Arbeitsumgebung bereit und was sind Aufgaben und Rollen?

**7.0.8.**
Wozu dienen Formulare? Warum besteht bei einem generalisierten Formularsystem die gefahr, das das ganze System mit Formularen aufgebaut wird?

**7.0.9.**
Wie unterscheiden sich Werkzeug und Automat?


7.1 Umsetzung
-------------

**7.1.1.**
Wie wird die Werkzeug-/Materialkopplung umgesetzt? Zu welchen Abhängigkeiten führt dies?

**7.1.2.**
[DP] Wie unterscheiden sich Composite und Decorator Pattern?

**7.1.3.**
Stellen Sie die Varianten "Aspekte über Vererbung" und Aspekte über Adapter oder Decorator" einander gegenüber. Welche Vererbungsbeziehung wird beim Zweiteren mit einer Delegation ersetzt?

**7.1.4.**
Wie wird Funktion und Interaktion getrennt? Wozu?

**7.1.5.**
[DP] Wie baut man komplexe Werkzeuge, die aus einfacheren zusammengesetzt sind?

**7.1.6.**
Wie ist die Rückkoppelung zwischen Funkton und Interaktion aufgebaut?

**7.1.7.**
Was ist "Feedback FK-IAK"?

**7.1.8.**
Wie werden Handhabung und Präsentation getrennt?

**7.1.9.**
Welche Möglichkeiten gibt es, um Fachwerte (Values) zu implementieren?

**7.1.10.**
Wie werden fachliche und technische Behälter umgesetzt? Wie funktioniert das Laden von Objekten?

**7.1.11.**
Wie werden Formularsysteme aufgebaut? Wozu sollten Sie verwendet werden, und wozu nicht?

**7.1.12.**
[DP] Wie kann man ein Embedded System mit einem technischen Automat an ein WAM Anwendungssyszem koppeln?

**7.1.13.**
Wie werden Domain Services umgesetzt? Wie sieht die Service Architektur aus?

**7.1.14.**
Wie wird das Environment umgesetzt?


8 Eclipse
=========

**8.0.1.**
Erklären Sie, was "Extension Points" in Eclipse sind und wozu sie eingesetzt werden.

**8.0.2.**
Eclipse setzt diverse Patterns ein. Erklären Sie anhand des angegebenen Einsatzgebietes, wie das Pattern eingesetzt und aufgebaut wird:

a) Singleton: PlatformUI.getWorkbench()
b) Proxy: IResource
c) Bridge: ResourceInfo (Resource --> ResourceInfo)
d) Adapter: IContentProvider (Domain <--> Viewer)
e) Observer: WorkspaceChangelistener
f) Strategy:  FormLayout/GridLayout/RowLayout
g) Command: IAction
h) Template Method: Refactoring Language Toolkit LTK
i) Composite: LTK Change/CompositeChange
j) Memento: LTK History
k) Visitor: ASTVisitor des CDT

**8.0.3.**
Welches Konzept wendet Eclipse4 anstelle Singletons an? Warum führt dies zu besserer Testbarkeit?


9 JUnit
=======

**9.0.1.**
Wie wird das "Command Pattern" in JUnit eingesetzt?

**9.0.2.**
Wie wird das "Template Method Pattern" eingesetzt?

**9.0.3.**
Was ist das "Collecting Parameter Patter"? Wie funktioniert es und wie/wozu wird es in JUnit eingesetzt?

**9.0.4.**
Wozu wird Reflection eingesetzt? Wie verbessert dies die Benutzbarkeit?

**9.0.5.**
Wozu wird das Composite Pattern bei JUnit eingesetzt?

**9.0.6.**
Mit dem Decorator Pattern kann JUnit erweitert werden. Wie funktioniert dies?

**9.0.7.**
Warum sollte ein Test normalerweise nur einmal laufen gelassen werden (mit den selben Parametern)?

**9.0.8.**
Wie ist JUTLAND aufgebaut? Warum ist es so schlank?

**9.0.9.**
Fit parst Html, setzt dazu jedoch keine Knoten und Tags ein sondern "Parse". Wie funktioniert es? Nennen Sie Vor- und Nachteile der Strategie.

**9.0.10.**
Cute kommt ohne Vererbung und Interfaces aus. Wie funktioniert es?

**9.0.11.**
Erklären Sie das "Policy-based Design Pattern". Stellen Sie es Dynamischer Polymorphie gegenüber.

**9.0.12.**
Was ist "Curiously recuring template parameter"?


10 Parallel Programming
=======================

**10.0.1.**
Erklären Sie die Abkürzungen UE und PE.

**10.0.2.**
Erklären Sie die Architekturen SISD, SIMD, MIMD und MISD.

**10.0.3.**
Wie weiter wird bereits innerhalb einer CPU (singlecore) parallelisiert?

**10.0.4.**
Erklären Sie "Task Decomposition" und "Data Decomposition".

**10.0.5.**
Erklären Sie die Vorgehensweise zur Gruppierung und Ordnung von Tasks sowie zum Data Sharing.

**10.0.6.**
Was ist "Pipeline Processing"?

**10.0.7.**
Wie funktioniert "Divide and Conquer"?

**10.0.8.**
Wie berechnen Sie parallel Summen von Zahlen?

**10.0.9.**
Was ist "geometric Decomposition"?


11 Flyweight & Singleton
========================

**11.0.1.**
Welche Vor- und Nachteile bringt das Flyweight mit sich?

**11.0.2.**
Flyweight shared Objekte und benutzt einen externen State. 
Welche Umgebungsbedingungen müssen erfüllt sein, damit FW wirklich angewendet werden kann?

**11.0.3.**
Aus welchen Patterns setzt sich FW zusammen?
Erklären Sie jedes davon.

**11.0.4.**
Welche Probleme soll Singleton lösen?

**11.0.5.**
Welche Probleme bringt Singleton mit sich?

**11.0.6.**
Wie kann ein Singleton ersetzt werden?

**11.0.7.**
Was ist Monostate? Wo liegen die Vor- und Nachteile?

**11.0.8.**
Was ist CRTP? Wie wird es eingesetzt?








