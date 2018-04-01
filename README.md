# Programmieren 2

_Pflichtmodul im [Bachelorstudiengang Wirtschaftsinformatik](https://www.fh-rosenheim.de/technik/informatik-mathematik/wirtschaftsinformatik-bachelor/) an der [Hochschule Rosenheim](https://www.fh-rosenheim.de)._

## Organisatorisches

**Vorlesungstermin**: Mittwochs, 8:00 R0.02

**Übungen**: Mittwochs, 2./4./5. Stunde, A0.03; Tutor: [Lukas Grams](https://github.com/gramsimamsi) (@sinflugram)

**Kommunikation**: via [Mattermost](https://inf-mattermost.fh-rosenheim.de/wif-prg2/channels/town-square) ([einschreiben](https://inf-mattermost.fh-rosenheim.de/signup_user_complete/?id=wp3dau8xmigxtmf93z5ixur1ta))

**Wichtige Termine**:

- **20.-30. April:** Prüfungsanmeldung im OSC (incl. PStA)
- **25. Mai:** Einführung in das Contestsystem der PStA (persönliche Anwesenheit erforderlich!)
- **4. Juli.:** Testat zur PStA (statt Übung)


## Leistungsnachweis

Der Leistungsnachweis ist aufgeteilt in eine 

- (unbenotete) praktische Studienarbeit (PStA), abzulegen während des Semesters (mit Abschlusstestat)
- schriftliche Prüfung (SP, 90 Minuten) am Ende des Semesters


## Empfohlene Literatur

- [Offizielle Java Dokumentation](https://docs.oracle.com/javase/9/)
- Ullenboom, C: [Java ist auch eine Insel](https://www.amazon.de/Java-auch-eine-Insel-Java-Entwickler/dp/3836258692/), 2017. ([Online verfügbar!](http://openbook.galileocomputing.de/javainsel))
- Bäckmann, M: [Objektorientierte Programmierung für Dummies](https://www.amazon.de/Objektorientierte-Programmierung-Dummies-Marcus-B%C3%A4ckmann/dp/3826629841/), 2002. _Das Buch ist für C++, die Methodik aber identisch zu Java._
- Gamma, E et al.: [Design Patterns](https://www.amazon.com/Design-Patterns-Object-Oriented-Addison-Wesley-Professional-ebook/dp/B000SEIBB8), 1994. (Das Buch ist in englischer und deutscher Fassung in der Bibliothek vorhanden).


## Inhalt
- **21. März: Professionelle Softwareentwicklung** ([Einführung](00-einfuehrung/), [Skript](01-professionelle-softwareentwicklung/), [Übung 1](https://github.com/hsro-wif-prg2/tutorial), [Übung 2](https://github.com/hsro-wif-prg2/example))
	
	Nach ein paar organisatorischen Dingen widmen wir uns dem Handwerkszeug professioneller Softwareentwicklung.
	Wir wiederholen Spezifikation mit UML, Versionierung mit git, Tests und Ausnahmebehandlung.

- **28. März: Liste als sequenzielle Datenstruktur** ([Skript](02-linked-list/), [Übung](https://github.com/hsro-wif-prg2/uebung01))

	Bisher haben wir größere Mengen von gleichen Objekten in Feldern (Arrays) gespeichert, welche aber in ihrer Größe in Java unveränderlich sind.
	Wir erarbeiten uns nun mit Hilfe von Objektorientierung eine dynamische Datenstruktur, welche nach Bedarf wachsen und schrumpfen kann, und so Daten effizient verwaltet.

- **4. April: Set als Menge eindeutiger Elemente** ([Skript](/03-tree-set/))

	Eine Liste speichert Daten sequenziell ab, achtet dabei aber nicht auf Duplikate.
	Ein _Set_ (aus dem engl. _set:_ Menge, Gruppe) ist ein Containertyp, welcher der mathematischen Menge nachempfunden ist: jedes Element kann genau einmal vorkommen, und es gibt keine Ordnung (Reihenfolge); ein Element ist entweder enthalten oder nicht.
	Zur Implementierung lernen wir den Binärbaum kennen, eine weitere wichtige Datenstruktur der Informatik.

- **11. April: Generics**

	Bisher waren die Containerklassen entweder für genau einen Datentyp, oder für die `Object`, welche für jedes Objekt verwendet werden kann.
	_Generics_ erlauben es nun mit beliebigen _aber festgelegten_ Datentypen zu arbeiten.
	Wir lernen ausserdem die Interfaces `Comparable` und `Comparator` kennen.

- **18. April: Map als generischer assoziativer Container**

	Eine Liste ist sequenziell mit potentiellen Duplikaten, ein Set ist duplikatfrei, aber ohne Reihenfolge.
	Eine _Map_ (aus dem engl. _map_: Abbildung) ist ein assoziativer Container, welcher einem Schlüssel (_key_) eindeutig einen Wert (_value_) zuordnet.

- **25. April: Annotationen; Einführung in die PStA**
	
	Nach einem kurzen Exkurs zum Thema Annotationen und deren Einsatzgebiete gibt es eine kurze Einführung in die PStA.

- **2. Mai: Iteratoren**

	Arrays und Listen verfügen über einen Indexoperator (`[]` bzw. `get(int)`) welcher verwendet werden kann um alle Elemente zu besuchen.
	Der _Iterator_ abstrahiert dieses Prinzip: Bereitgestellt vom Container selbst, ist er ein Hilfsobjekt mit dem jedes Element des Containers besucht werden kann.

- **9. Mai: Rekursion**

	Ging es um das Abarbeiten von Daten bzw. implementieren von Algorithmen, so gingen wir bisher meist iterativ vor, also mit `for` bzw. `while`.
	Rekursion ist nun ein Mittel, bei der eine Methode sich selbst wieder (mit veränderten Argumenten) aufrufen, und so ohne `for` bzw. `while` auskommen.

- **16. Mai: Sortieren**
	
	Gewappnet mit Datenstrukturen, Iteration und Rekursion erarbeiten wir Algorithmen zum Sortieren von Daten.
	Wir begegnen wieder den Interfaces `Comparable<T>` und `Comparator<T>`, welche die Vergleichsoperation abstrahieren.

- **23. Mai: Arbeiten mit Containern**

	Wir lernen die Containerklassen der Java Bibliothek kennen, und wie man sie nutzt um schnell (und übersichtlich) Daten zu verarbeiten.
	Klassischerweise ist die Datenverarbeitung hier in drei Schritten zu machen: filtern, abbilden und reduzieren.

- **30. Mai: Rückblick**
	
	Wir fassen die wichtigsten Datenstrukturen, Algorithmen und Konzepte zusammen und besprechen weitere Beispiele.

- **6. Juni: Vererbung**

	Bisher waren unsere Klassenbeziehungen vorwiegend strukturell bzw. funktional: Ein Monat besteht aus Tagen, ein Auto aus Bauteilen, usw.
	_Vererbung_ erlaubt es nun verwandschaftliche Beziehungen zu modellieren, und so Gemeinsamkeiten in Oberklassen zu bündeln.
	So sind z.B. sowohl Audis als auch BMWs im Grunde genommen _Autos_, doch gibt es sowohl geteilte Eigenschaften als auch spezielle.

- **13. Juni: Abstrakte Basisklassen**
	
	Abstrakte Basisklassen sind ein weiteres Syntaxmittel, um verwandschaftliche Beziehungen zu beschreiben.
	Da abstrakte Klassen nicht instanziiert werden können, sind sie im Grunde ähnlich zu Schnittstellen (_Interfaces_), erlauben aber genauere modellierung der Sichtbarkeiten.

- **20. Juni: Parallele Verarbeitung**
	
	Folgten unsere Programme bisher einem vorgesehenen Ablaufplan, so erlauben _Threads_ die parallele Verarbeitung von Daten.
	Wir beginnen mit der Basisimplementierung und erarbeiten einige knifflige Situationen.

- **27. Juni: Design Patterns**
	
	Professionelle Softwareentwicklung greift oft auf Entwurfsmuster (_design pattern_) zurück.
	Wir wiederholen einige welche wir bereits kennen gelernt haben, und erarbeiten eine Systematik für weitere Muster.

- **4. Juli: Zusammenfassung**


_Abboniere das [https://github.com/hsro-wif-prg2/hsro-wif-prg2.github.io Repository](https://github.com/hsro-wif-prg2/hsro-wif-prg2.github.io) um bei Updates benachrichtigt zu werden._
