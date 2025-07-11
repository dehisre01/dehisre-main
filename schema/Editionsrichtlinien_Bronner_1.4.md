Editionsrichtlinien der digitalen Edition des Reisejournals Franz Xaver Bronners


Version 1.4


### 1. Einleitung


Die vorliegenden Editionsrichtlinien dienen der Erstellung einer digitalen Edition des Reisejournals Franz Xaver Bronners aus dem 19. Jahrhundert. Ziel ist es, eine originalgetreue, wissenschaftlich fundierte und benutzerfreundliche Edition bereitzustellen, die sowohl den transkribierten Text als auch Faksimiles der Handschrift in einer synoptischen Ansicht integriert.


Die Übertragung des Textes in die digitale Form berücksichtigt den von der DFG empfohlenen Standard für Textauszeichnung und -archivierung in TEI-XML (DFG: Förderkriterien für wissenschaftliche Editionen in der Literaturwissenschaft, 2015). Die Richtlinien basieren auf den Vorgaben der Text Encoding Initiative (TEI) und dem darauf aufbauenden Basisformat des Deutschen Textarchivs (DTABf).


Die **Edition** umfasst eine diplomatische Wiedergabe des Textzeugen und ermöglicht den Vergleich mit seitenweise verknüpften Faksimiles der Originalhandschrift. Für die textkritische Wiedergabe sind zwei Textversionen verfügbar: eine diplomatische Transkription und eine konstituierte Textversion, in der der originale Zeilenfall aufgelöst wird und die Streichungen und Korrekturen des Textzeugen emendiert werden. (Siehe § 3.2.2.)


Die **Transkription** des Reisejournals Bronners wird originalgetreu auf Basis der Handschrift des 19. Jahrhunderts wiedergegeben. Folgende Aspekte werden dabei berücksichtigt:


- **Zeilenfall, Silbentrennung, Paginierung**: Originalgetreu wiedergegeben

- **Kopfdaten, Kustoden und Bogensignaturen**: Inklusive der originalen Gestaltung

- **Faksimile-Verknüpfung**: Jede Seite der Transkription ist mit dem entsprechenden Faksimile verknüpft

Der Wortlaut wird zeichengetreu unter Berücksichtigung bedeutungstragender Eigenheiten der handschriftlichen Gestaltung wiedergegeben. Dies schließt Streichungen und Korrekturen als solche ein. Schreibfehler und Zeichensetzungen der Handschrift werden übernommen und nicht emendiert. Zusätzlich werden marginal fortgeführte Sätze, supralineare Ergänzungen, Zeichnungen und Listen in den Text eingefügt.


Die **Orthographie** wird in ihrer zeittypischen Heterogenität wiedergegeben, einschließlich wechselnder Groß- und Kleinschreibung, unterschiedlicher Wortabstände bei Komposita sowie der eigenwilligen Interpunktion.


**Unleserliche** Wortteile sind mit einem [?] gekennzeichnet, nicht mehr entzifferbare ganze Wörter werden durch [unleserlich] bzw. [schwer lesbar] ersetzt. Konjekturen werden wiedergegeben (Siehe § 3.2).


Die im Original vorkommenden **Zeit- und Maßangaben** sowie **Währungszeichen** werden durch die entsprechenden Symbole oder gebräuchliche Abkürzungen dargestellt und in den Annotationen aufgelöst.


Die Edition enthält ein **Personen- und Ortsregister**, das als Hilfsmittel dient, um die Identität von Personen zu verifizieren und die räumlichen Bewegungen Bronners nachvollziehen zu können (Siehe § 3.3 und § 4).


Das Personenregister informiert über Namen (einschließlich Geburts- und Ehenamen), Lebensdaten, berufliche Stellung sowie die wichtigsten Verwandtschaftsbeziehungen. Zur Identifikation der in den Reiseaufzeichnungen Bronners erwähnten Personen wurden neben gängigen auch entlegenen biographischen Nachschlagewerken sowie Kirchenbücher, Staats- und Hofkalender, Adressbücher, Universitäts- und Schulmatrikel und weitere Quellen herangezogen. Zusätzlich wurde auf zeitgenössische und aktuelle Spezialliteratur zurückgegriffen. Das Personenregister führt die mutmaßlich korrekte oder zumindest gebräuchlichste Namensform auf.


Nicht alle Personen konnten ermittelt werden. In diesen Fällen beschränkt sich das Register darauf, die Personen mit ihrem Namen und entsprechend dem Familienstand aufzunehmen oder die berufliche Zugehörigkeit oder den militärischen Rang zu nennen. Zudem wird nach Möglichkeit der Ort angegeben, an dem die Person lebte oder mit Bronner in Kontakt trat.


Im Register sind nicht nur Einzelpersonen, sondern auch „Personenvereinigungen“ wie Vereine, Kollegien und Senate aufgeführt, jeweils unter dem Ort ihrer Ansässigkeit.


Die Ortsnamen im **Ortsregister** werden in der Regel in der heute üblichen deutschen Schreibweise dargestellt. Städte und Dörfer, die zur Zeit Bronners eigenständige Einheiten bildeten, erhalten jeweils ein eigenes Lemma. Darüber hinaus sind Schlösser, Burgen, Landgüter, Poststationen, Flüsse, Gebirge sowie Territorien und Staaten aufgenommen, jeweils in der zum Zeitpunkt der Erwähnung in der Reisebeschreibung gültigen Form.


  

### 2. Metadaten der digitalen Edition


#### 2.1. Textsorten


Die Edition umfasst folgende Textsorten:


- Reisebericht Franz Xaver Bronners:

- Reinschrift Hinreise

- Entwurf Hin- und Rückreise

Die nachfolgenden Kodierungsrichtlinien folgen den Besonderheiten handschriftlicher Manuskripte.


#### 2.2. Standardisierte Metadaten


Die Edition verwendet standardisierte Metadatenformate wie Dublin Core und METS, um eine optimale Auffindbarkeit und Interoperabilität zu gewährleisten. Alle relevanten Metadaten werden im TEI-Header definiert.


#### 2.3 Bibliografische Angaben


Vollständige bibliografische Angaben zur Edition umfassen:


- Editionstitel und Autor

- Herausgeber und Bearbeiter

- Erscheinungsort der Edition

- Erscheinungsjahr und Version

- Publikationsformat

- Herkunft des Textzeugen

- Zusammenfassung der relevanten bibliografischen Details

  

### 3. Textauszeichnung


Die Textauszeichnung basiert auf TEI-XML und folgt den Empfehlungen des Deutschen Textarchivs. Unterschiedliche Strukturelemente werden präzise kodiert, um eine konsistente und durchsuchbare Datenbasis zu schaffen.


#### 3.1 Strukturelemente


- **Seiten- und Blattnummer**

Seitenwechsel werden durch das Element ```<pb>``` (pagebreak) gekennzeichnet. Das Attribut @n kennzeichnet die Seitenzahl- bzw. die Paginierung des Blattes.


Bsp.: 
```
<pb n=“5v“/>
```


Der Link zum Digitalisat ist im Attribut @facs (facsimile) angegeben. Als Link werden Permalinks der bestandshaltenden Institution verwendet.


Bsp.: 
```
<pb n="5v" facs="http://..."/>
```
  

Die Seitenzahl wird durch das Element ```<fw>``` angegeben. Es enthält die Nummer als Text und trägt die Elemente @hand und @type.


  

Bsp.: 
```
<fw hand= "#bronner" type= "folNum">123</fw>
```


- Absätze

Absätze werden mit dem Element ```<lb/>``` (paragraph) codiert.


Bsp.:

```
<p>
  [Textinhalt]
</p>
```


- Zeilenumbrüche

Zeilenumbrüche werden mit dem Element ```<lb/>``` (line beginning) am Anfang einer Zeile codiert.


```
<lb/>[Textinhalt]
```


- Leere Seiten und unleserliche Stellen

Leere Seiten werden mittels ```<gap/>``` Element ausgezeichnet. Es folgt direkt auf den entsprechenden Seitenwechsel mit Angabe der Seitenzahl (```<pb/>```). Mit den Attributen @unit und @quantity des Elements ```<gap/>``` werden zusätzlich Einheit und Menge der leeren Seite definiert, ergänzt wird dies mit dem Attribut @reason. Mehrere leere Seiten hintereinander werden einzeln codiert.


Bsp.:

```
<pb n="132v"/>
<gap unit="pages" quantity="1" reason="empty"/>
```

  

Ebenfalls mit ```<gap/>``` ausgezeichnet werden unleserliche oder zerstörte Textstellen. Unter @unit werden die nicht lesbaren Segmente definiert:



|@unit  |Bedeutung  |
|--|--|
|chars  |Zeichen  |
|lines  |Zeilen  |
|pages  |Seiten  |
|words  |Wörter  |

Das Attribut @reason beschreibt zudem den Grund für die Unleserlichkeit:


| @reason |Bedeutung  |
|--|--|
|lost  |Zerstörung/Verlust |
|illegible  |unleserlich  |
|covered  |durch Überschreibung schwer leserlich  |
|empty  |Leere Seite  |

- Listen

Listen werden als solche transkribiert und mit dem Element ```<list>``` ausgezeichnet. Die einzelnen Aufzählungspunkte oder Zeilen werden mit dem Element ```<item>``` umschlossen. Titel werden, wenn vorhanden, durch das Element ```<head>``` markiert.


Bsp.:

```
<list>
  <item>[Erster Punkt]</item>
  <item>[Zweiter Punkt]</item>
</list>
```


- Tabellen

Tabellen werden als solche transkribiert und mit dem Element ```<table>``` ausgezeichnet.



Bsp.:

```
<table>
  <row>[Erster Zeile]
    <cell>[Erste Zelle Erste Zeile]</cell>
    <cell>[Zweite Zelle Erste Zeile]</cell>
  </row>
  <row>[Zweite Zeile]
    <cell>[Erste Zelle Zweite Zeile]</cell>
    <cell>[Zweite Zelle Zweite Zeile]</cell>
  </row>
</table>
```

- Zeichnungen und Abbildungen

Zeichnungen werden als solche transkribiert und mit dem Element ```<figure>``` ausgezeichnet.
  

Bsp.:

```
<figure facs="Dateiname Abbildung">
  <p>[Bildunterschrift im Manuskript]</p>
  <figureDesc>[Bildbeschreibung Bearbeiter:in]</figureDesc>
</figure>
```


#### 3.2 Textbearbeitung


Unterschieden wird zusätzlich in: Textbearbeitungen durch Autor:innen (3.2.1) und Textbearbeitungen durch Herausgeber:innen (3.2.2).


#### 3.2.1 Textbearbeitungen des Autors


- Ergänzungen

Ergänzungen werden durch das Element ```<add>``` (addition) gekennzeichnet, das Attribut @place gibt zusätzlich die Position dieser Ergänzung an. Ergänzungen können sich unter- oder oberhalb der Zeile sowie am linken oder rechten Rand befinden.


Bsp.:

```
<add place="interlinear">[ergänzter Text]</add>
```

| @place |Bedeutung |
|--|--|
|superlinear  |über der Zeile  |
|interlinear  |unter der Zeile  |
|across  |über den ursprünglichen Text  |
|left   |am linken Rand   |
|right   |am rechten Rand   |
|mTop   |am oberen Rand   |
|mBottom   |am unteren Rand   |  

- Streichungen

Gestrichener Text wird mit dem Element ```<del>``` (deletion) ausgezeichnet und soweit lesbar transkribiert, hierbei werden zusätzlich alle Textphänomene, Auflösungen, Normalisierungen und Korrekturen berücksichtigt und entsprechend ausgezeichnet.


Bsp.:

```
<del rendition="#s">durchgestrichen</del>
```

Das Attribut @rendition gibt Auskunft über die Art der Streichung:


|@rendition  |Bedeutung  |
|--|--|
|#ow  |ursprünglicher Text überschrieben  |
|#s  |Textstelle durchgestrichen  |
|#erased  |Zerstörter bzw. ausradierter Text  |
  

- Korrekturen

Korrekturen durch Autor:innen werden als Substitutionsprozess innerhalb des Elements ```<subst>``` (substitution) dargestellt. Dieser Prozess besteht aus zwei Teilen: Dem Löschungsvorgang mittels des Elements ```<del>``` (deletion) und der Ergänzung des neuen Textes durch das Element ```<add>``` (addition). Angaben zur Art der Streichung und Art der Einfügung werden, wie unter Streichung und Ergänzung beschrieben, mit den Attributen @rendition und @place hinzugefügt.


Bsp.:

```
<subst>
   <del rendition="#ow">f</del>
   <add place="across">t</add>
</subst>
```

- Typographische Besonderheiten

Textteile mit typographischen Besonderheiten werden mit dem ```<hi>```-Element ausgezeichnet:


Bsp.:

```
<hi rendition="#u">unterstrichen</hi>
```
  

Das Attribut @rendition spezifiziert die Art der typographischen Besonderheit:

|@rendition  |Bedeutung  |
|--|--|
|#sub  |Tiefstellung  |
|#sup  |Hochstellung  |
|#u  |Unterstreichung  |
|#uu   |doppelte Unterstreichung   |

#### 3.2.2 Textbearbeitungen der Herausgeber:innen


  

- Auflösung

Zu Ergänzungen durch Herausgeber:innen zählen u. a. die Ergänzung abgekürzter Wörter. Herausgeber:innen können Wörter auflösen, um beispielsweise eine bessere Lesbarkeit zu erzielen. Abkürzungen und ihre Auflösung werden mit Hilfe von ```<choice>``` codiert, näher definiert wird die Auflösung mittels der Kindelemente ```<abbr>``` (abbreviation) und ```<expan>``` (expansion). Im ```<abbr>```-Element wird die Abkürzung der Vorlage entsprechend festgehalten, im ```<expan>```-Element wird die Ergänzung oder Auflösung notiert.


Bsp.:

```
<choice><abbr>Jan.</abbr><expan>Januar</expan></choice>
```


- Fehlende Wörter, Buchstaben oder Satzzeichen

Fehlende Wörter oder Satzzeichen werden mithilfe des ```<supplied>``` Elements ausgezeichnet. Über das Attribut @cert (certainty) wird zusätzlich angegeben, mit welcher Wahrscheinlichkeit die vorgenommene Erweiterung zutrifft – „high“ steht dabei für hoch und „low“ für niedrig.


Die in seltenen Fällen erfolgte Ergänzungen dienen der besseren Lesbarkeit des Textes. Ergänzungen sind genau abzuwägen und können sich über Buchstaben und Satzzeichen oder auch ganze Wörter erstrecken.


Bsp.:


```
<supplied cert="high">l</supplied>
```



- Korrekturen

Schreibfehler werden durch die Herausgeber:innen nicht korrigiert. Die fehlerhaften Textstellen werden entsprechend der Vorlage transkribiert und, wenn notwendig (siehe oben), ausgebessert. Solche Fehlerkorrekturen werden mit dem ```<choice>```-Element umschlossen. Das fehlerhafte bzw. fehlende Wort oder Satzzeichen wird mit ```<sic>``` ausgezeichnet und die Korrektur durch das ```<corr>```-Element (correction) ergänzt. Mit dem Attribut @cert wird zusätzlich angegeben, mit welcher Wahrscheinlichkeit eine Korrektur zutrifft, unterschieden wird dabei in „high“ und „low“.


Bsp.:


```
<choice><sic>Der</sic><corr cert="high">Das</corr></choice>
```



Ein weiteres Beispiel für fehlerhafte Textstellen im Text ist die irrtümliche doppelte Setzung desselben Wortes. Die damit verbundene Korrektur durch Streichung eines Wortes (oder mehrerer Wörter) durch die Herausgeber:innen, wird im Element ```<choice>``` vorgenommen. Das Kindelement ```<sic>``` kennzeichnet das zu streichende Wort, die Streichung selbst wird innerhalb des Kinelements ```<corr>``` mit dem Attribut @type, welches den Wert „deleted” trägt, ausgezeichnet.


Bsp.:


```
<choice><sic>Baum</sic><corr type="deleted"/></choice>
```


- Unsichere Transkription

Für nicht lesbare oder schwer lesbare Textteile wird das Element ```<unclear>``` verwendet. Dies trifft zu, wenn z. B. durch Überschreibung oder Verschmutzung die Lesbarkeit des Textes eingeschränkt ist. Mit ```<unclear>``` wird eine gewisse Unsicherheit in der Transkription gekennzeichnet. Die Ursache der Unsicherheit kann über das Attribut @reason mit den Werten „illegible“ oder „covered“ näher beschrieben werden. Mit welcher Wahrscheinlichkeit die Transkription zutrifft, wird mit dem Attribut @cert und den Werten „high“ oder „low“ angegeben.


#### 3.3 Auszeichnung von Entitäten


- Personennamen

Personen werden durch das Element ```<persName>``` gekennzeichnet. Das Attribut @key verknüpft das Element mit dem korrespondierenden Element im Register. Als Wert trägt es die xml:id des Registereintrags.


Bsp.:
```
<persName key="per_fxb_1234">Jungh</persName>
```

- Ortsnamen

Orte werden durch das Element ```<placeName>``` gekennzeichnet. Das Attribut @key verknüpft das Element mit dem korrespondierenden Element im Register. Als Wert trägt es die xml:id des Registereintrags.


Bsp.:

```
<placeName key="ort_fxb_1234">Aarau</placeName>
```



- Werktitel

Titel der literarischen und künstlerischen Werke werden mit dem Element ```<bibl>``` ausgezeichnet.


Bsp.:

```
<bibl>Titel des Werks</bibl>
```


  

- Datumsangaben

Datumsangaben sind für die Nachvollziehbarkeit des Reiseverlaufs von großer Bedeutung und werden deshalb im Text ausgezeichnet. Datumsangaben erhalten das Element ```<date>```, das maschinenlesbare Datum wird dabei im Format JJJJ-MM-TT in den Attributen @when, @from und @to sowie @notBefore oder @notAfter notiert.

  

Folgenden Erscheinungsformen sind möglich:



| Datumsangabe |Beispiel  |
|--|--|
|genaues Datum  |```<date when="1772-12-21">21. Dezember 1772</date>```|
|genaue Zeitspanne  |```<date from="1731-11-11" to="1741-09-11">11. November 1731 bis 11. September 1741</date>```|
|ungefährer Zeitraum  |```<date notBefore="1804-05-01" notAfter="1804-05-16">Erste Hälfte Mai 1804</date>```|
  

Im Attribut @cert kann mit den Werten high bzw. low die Wahrscheinlichkeit angegeben werden, mit der die Datumsangabe zutrifft. In dem Attribut @calendar wird definiert, ob sich die Datumsangabe nach dem Julianischen Kalender (#julian) oder dem Gregorianischen Kalender (#gregorian) richtet.


  

- Zeitangaben

  

Zeitangaben werden über das Element ```<time>``` definiert. Die Attribute verhalten sich dabei ähnlich wie bei Datumsangaben, siehe hierfür die Tabelle unter “Datumsangaben”.


  

@dur Angabe einer Zeitspanne: 1 Stunde, 1 Woche


  

@when Angabe der genauen Zeit und der Zeitzone Bsp.: +01:00 Berlin


  

@notBefore @notAfter ungefähre Zeitangabe


  

- Maßangaben

Maßangaben werden über das Element ```<measure>``` gekennzeichnet und durch die folgenden Attribute ergänzt:

  

@unit bezeichnet die erwähnte Einheit, wie z.B. Rubel. Mittels @type wird die Art der Maßeinheit näher beschrieben, zur Verfügung stehen hier “currency” und “dimension”. Unter @quantity wird die genaue Menge festgehalten.


  

Bsp.:

```
<measure type=”currency” unit=”Rubel” quantity="4">4 Papier-Rubeln</measure>
```


### 4. Register


Die Edition enthält umfassende Personen- und Ortsregister, die als Hilfsmittel zur Verifikation der Identität von Personen und zur Nachvollziehbarkeit der räumlichen Bewegungen von Bronner dienen. Diese alphabetisch sortierten Register bieten eine systematische Übersicht über alle relevanten Personen und Orte, die im Rahmen der Edition erwähnt werden.


Die Registereinträge werden als Liste geführt, und werden in einem ```<listPlaces>``` respektive ```<listPersons>``` als Elternelement für alle Orte respektive Personen zusammengefasst.


#### 4.1 Personenregister


Das Personenregister erfasst Informationen zu allen im Text erwähnten Personen, einschließlich ihrer Namen, Lebensdaten, beruflichen Tätigkeiten sowie relevanter familiärer Verbindungen. Jeder Eintrag besteht aus einem ```<person>``` Element, welches als @xml:id eine ID aufweist, die eine eindeutige Verknüpfung zu den Vorkommnissen im Editionstext erlaubt.


Bsp.:

```
<person xml:id="per_fxb_1234">[Personendaten]</person>
```

  

#### 4.1.1 Erfasste Inhalte


- Personennamen

Die vollständigen Namen der Personen, einschließlich Geburtsnamen, Ehenamen oder anderer bekannter Namensvarianten. Diese werden im ```<persName>```-Element codiert, mit dem Attribut @type, das zwischen kanonisierten Namen (reg), der einmal vorkommt und alternativen Namen (alt), die beliebig viele Vorkommen haben dürfen, differenziert. Es gibt die Möglichkeit über das Attribut @subtype mit dem Wert “birthname” den Geburtsnamen anzugeben.


Bsp.:

```
<persName type="reg">
<surname>Schorcht</surname>
<forename>Karoline Maria Friederike</forename>
</persName>
<persName type="alt" subtype="birthname">
<name>Wieland</name>
</persName>
```

  

- Titel

Namenszusätze und Titel werden, falls vorhanden und bekannt, im Element ```<roleName>``` ausgezeichnet. Adelsprädikate wie “von" werden hinter den Vornamen im Element ```<forename>``` vermerkt, um die alphabetische Sortierung nach Nachnamen nicht zu korrumpieren.


Bsp.:

```
<persName type="reg">
<surname>Romanov</surname>
<forename>Alexander Pavlovič</forename>
<roleName type="nobility">
<name>Russischer Kaiser</name>
</roleName>
</persName>
<persName type="alt">
<name>Alexander I.</name>
</persName>
```


- Lebensdaten

Geburts- und Todesdaten werden durch die Elemente ```<birth>``` und ```<death>``` kodiert, die als Kindelemente von ```<person>``` erscheinen und das Datum als Text enthalten, sowie als Wert des Attributs @when.


Bsp.:

```
</person> [...]
<birth when= "1777">1777</birth>
<death when= "1825">1825</death>
[...]</person>
```


- Berufliche Stellung

Die berufliche Position der Person wird durch das Element ```<occupation>``` ausgezeichnet.


Bsp.:

```
<occupation>Schriftsteller</occupation>
```


- Biologisches Geschlecht

Das (biologische) Geschlecht der Person wird durch das Element ```<sex>``` erfasst und enthält den Deutschen Wert als Text. Außerdem wird es über das Attribut @value angegeben, mit den möglichen Werten “female” (weiblich), “male” (männlich) und “unknown” (unbekannt). Wir haben für keine im Register vorkommende Person Kenntnisse, die eine Zuschreibung zu einer Kategorie jenseits dieser Binarität sinnvoll erscheinen ließe.


Bsp.:

```
<sex value="male">männlich</sex>
```


- Unbekannte Personen: Aufnahme mit Namen, Familienstand oder militärischem Rang und, wenn möglich, dem Ort der Lebensführung oder Kontaktaufnahme mit Bronner.

Bsp.:

```
</person>
<person xml:id="per_fxb_198">
<persName type="reg">
<surname>...</surname>
<forename>...</forename>
</persName>
<birth>?</birth>
<death>?</death>
<sex value="female"/>
<occupation>Wirtin</occupation>
<note>Wirtin von Doblehn</note>
</person>
```


- GND-Eintrag

Wenn eine Person über eine GND-Nummer (Gemeinsame Normdatei) verfügt, wird diese Information im Element ```<idno>``` mit dem Attribut @type="uri" angegeben. Falls die Person keinen Eintrag in der GND hat, wird das -Element weggelassen.


Bsp.:

```
<idno type="uri">http://d-nb.info/gnd/12345678</idno>
```


#### 4.1.2 Annotationen und Kommentare der Herausgeber:innen


Zur Verifizierung und Ergänzung der biografischen Angaben werden verschiedene Quellen herangezogen, darunter:


- Biografische Nachschlagewerke

- Kirchenbücher

- Staats- und Hofkalender

- Adressbücher

- Universitäts- und Schulmatrikel

- Zeitgenössische und aktuelle Spezialliteratur

Kommentare und erklärende Annotationen werden in dem Element ```<note>``` untergebracht. Das ```<person>``` Element darf mehr als ein ```<note>``` Element beinhalten.


Bibliografische Referenzen und Quellen werden in dem Element ```<bibl>``` vermerkt. Ein ```<person>``` Element darf mehrere Quellenangaben beinhalten.


Ein vollständiger Personenregistereintrag kann wie folgt aussehen:


Bsp.:

```
<person xml:id="per_fxb_145"> 
    <idno type="uri">https://d-nb.info/gnd/118529919</idno> 
    <persName type="reg"> 
        <surname>Alexejewna</surname> 
        <forename>Elisabeth</forename> 
        <roleName>Russische Kaiserin</roleName> 
    </persName> 
    <persName type="alt" subtype=”birthname"> 
        <surname>Baden</surname> 
        <forename>Luise Marie Auguste von</forename> 
    </persName> 
    <birth when= "1779">1779</birth> 
    <death when= "1826">1826</death> 
    <sex value="female">weiblich</sex> 
    <occupation>Kaiserin</occupation> 
    <note>Kaiserin Elisabeth Alekseevna, Luise Marie Auguste Prinzessin von Baden. An der Seite des Kaisers Alexander I. von 1801 bis 1825 Kaiserin von Russland.</note> 
    <bibl>Elisabeth von Russland. Olivier, Daria. - München : Goldmann, 1979, Genehmigte Taschenbuchausg., 1. Aufl.</bibl> 
</person>
```


#### 4.2 Ortsregister


Das Ortsregister erfasst Informationen zu allen im Text erwähnten Orten, einschließlich ihrer Namen, Normdaten, Art des Ortes und Koordinaten. Jeder Eintrag besteht aus einem ```<place>```-Element, welches als @xml:id die ID aufweist, die eine eindeutige Verknüpfung zu den Vorkommnissen im Editionstext erlaubt.


Bsp.:

```
<place xml:id="ort_fxb_1234">[Ortsdaten]</person>
```


Die Art des Ortes wird optional über das Attribut @type spezifiziert. Die möglichen Werte für @type sind:


|@type  |Bedeutung  |
|--|--|
|street  |Straße  |
|building  |Gebäude  (Haus, Schloss, Landgut etc.)|
|sea  |Gewässer (See, Meer, Fluss etc.)  |
|mountain   |Berg und sonstige Erhöhung   |
|forest   |Wald, Bewaldung   |
|monument   |Monumente und Statuen   |
|district   |kleinere Verwaltungseinheit   |
|city   |Stadt   |
|country   |Land   |
|postalstation   |Poststation   |


Bsp.:

```
<place xml:id="ort_fxb_1234" type=”city”>[Ortsdaten]</place>
```


#### 4.2.1 Erfasste Inhalte


- Ortsnamen

Die Namen des Ortes nach aktueller deutscher Schreibweise wird im Element ```<placeName>```, mit dem Attribut @type und dem Wert “reg” angegeben. Alternative Schreibweisen und die Quellenbezeichnung – falls abweichend – werden durch ein zusätzliches ```<placeName>``` Element mit dem Attribut-Wert-Paar @type=”alt” kodiert.


Bsp.:

```
<placeName type="reg">Istanbul</placeName>
<placeName type=”alt">Konstantinopel</placeName>
<placeName type=”alt"> Kostantiniyye</placeName>
```


- Koordinaten

Koordinaten werden in den Elementen ```<location><geo>[Breitengrad], [Längengrad]</geo></location>``` angegeben. Für die Lokalisierung wurden gängige Datenbanken wie Geonames, Google Maps und Yandex Maps verwendet. Wenn die Quellenlage es zuließ, wurden auch eigene Lokalisierungen mit historischen Quellen vorgenommen. In diesen Fällen sind die Koordinaten oft nicht in Übereinstimmung mit den heutigen Stadtzentren. Entsprechende Lokalisierungen werden in Quellen und Kommentaren vermerkt.

```
<location>
    <geo>47.81252, 7.61016</geo>
</location>
```


- Adressen

Aktuelle Adressen werden im Element ```<address>``` angegeben, das ein Kindelement des Elements ```<location>``` ist.


```
<location> 
    <geo>[Breitengrad], [Längengrad]</geo> 
    <adress>Hauptstraße 2</address>
</location>
```
  

#### 4.2.2 Annotationen und Kommentare


Zur Validierung der Ortsnamen werden neben den aktuellen Normdatenbanken und Verzeichnissen auch historische Karten, Post- und Reise-Handbücher sowie Archivdokumente verwendet.


- Geonames-Eintrag

Wenn ein Ort über eine URI bei geonames.org verfügt, wird diese Information im Element  mit dem Attribut @type="uri" angegeben. Falls ein Ort keinen Eintrag in bei Geonames aufweist, wird das ```<idno>```-Element weggelassen.


Bsp.:

```
<idno type="uri">https://www.geonames.org/745042</idno>
```


- Erklärende Annotationen

Kommentare werden in dem Element ```<note>``` untergebracht. Über das Attribut type=”publication” wird explizit gemacht, falls es sich um einen Kommentar für die Printedition handelt. Das ```<place>``` Element darf mehr als ein ```<note>``` Element beinhalten.


Bsp.:

```
<note type="publication">Dorf mit ehemaligem Wasserschloss der Fuldaer Äbte aus dem 13. Jh., von dem heute nur noch die vier Ecktürme stehen. Der Ort gehörte 1810 zum Großherzogtum Frankfurt und hatte eine Poststation.</note>
```


- Quellen

Quellen werden in dem Element ```<bibl>``` vermerkt. Ein ```<place>``` Element darf mehrere Quellenangaben beinhalten.


Bsp.:

```
<bibl>Allgemeines Post- und Reise-Handbuch für Deutschland, Frankreich, die Schweiz, Italien, Spanien, Großbritannien, die nordischen Reiche und einige andere Länder. Nürnberg 1816, S. 34.</bibl>
<bibl>https://de.wikipedia.org/w/index.php?title=Neuhof_(bei_Fulda)&amp;oldid=236180281 (12.12.2023). Neuhof, Landkreis Fulda, in: Historisches Ortslexikon, 28. November 2022. https://www.lagis-hessen.de/de/subjects/idrec/sn/ol/id/6521 (12.12.2023).</bibl>
```


#### 4.2.3 Unterorte


Einige Orte sind eindeutig übergeordneten Orten zuzuordnen. Der offensichtlichste Fall hierfür sind Gebäude in einer Stadt. Um dies darzustellen können die übergeordneten Orte ein ```<placeList>``` Element führen, in welchem alle Unterorte nach oben beschriebenen Richtlinien eigene ```<place>``` Elemente darstellen. Unterorte können keine eigenen Unterorte haben, eine tiefere Schachtlung findet nicht statt.


Ein vollständiger Ortsregistereintrag kann wie folgt aussehen:


Bsp.:

```
<place xml:id="ort_fxb_217" type="city">
     <idno type="uri"> https://www.geonames.org/2903012</idno>
     <placeName type="reg">Höchstädt</placeName>
     <note>Marktplatz</note>
     <location>
         <geo>48.61137, 10.56712</geo>
     </location>
     <listPlace>
         <place xml:id="ort_fxb_2575" type="sea">
             <placeName type="reg">Altwasser (Höchstädt)</placeName>
             <note>Anfang des 19. Jh. wie heute Altwasser.</note>
             <location>
                 <geo>48.60149, 10.58783</geo>
             </location>
         </place>
         <place xml:id="ort_fxb_2576" type="building">
             <placeName type="reg">Aulingers Bleiche (Höchstädt)</placeName>
             <location>
                 <geo>48.60869, 10.56937</geo>
             </location>
         </place>
     </listPlace>
 </place>
```


### 5. Technische Standards und Benutzung


#### 5.1 TEI-XML


Die Kodierung folgt den TEI Guidelines, um eine strukturierte und nachhaltige Datenbasis zu gewährleisten. Die Textauszeichnung und Metadaten werden gemäß den Empfehlungen des Deutschen Textarchivs umgesetzt.


#### 5.2 Faksimile-Integration


Faksimiles werden als hochauflösende Bildformate eingebunden und seitenweise mit den transkribierten Texten verknüpft. Permalinks der bestandshaltenden Institutionen werden verwendet, um eine dauerhafte Verlinkung zu gewährleisten.


#### 5.3 Navigationsstruktur und Suchfunktionen


Die Online-Präsentation beinhaltet intuitive Navigationsmöglichkeiten durch Kapitel, Seiten und Registereinträge.


Im Rahmen der Online-Präsentation werden Suchfunktionen innerhalb der Transkription und der Faksimiles, einschließlich Volltextsuche und Suche nach Metadaten implementiert.


#### 5.4 Feedback-Mechanismen


Die Möglichkeit für Nutzer, Feedback zu geben oder Korrekturen vorzuschlagen wird durch den Email-Kontakt zum Editionsteam bzw. der für das Hosting zuständigen Institution realisiert.


### 6. Versionierung und Archivierung


Änderungen und Aktualisierungen der digitalen Edition werden auf GitHub (https://github.com/dehisre01/) dokumentiert, um Transparenz, Nachvollziehbarkeit und Aktualität dauerhaft sicherzustellen.


Eine umfassende und detaillierte Dokumentation der technischen Umsetzung sowie der angewandten Standards wird sowohl auf der offiziellen Website der digitalen Edition als auch über die Plattform Osmikon (https://www.osmikon.de/themendossiers) veröffentlicht, um die technische Transparenz und methodische Nachvollziehbarkeit zu gewährleisten.


Zur Sicherstellung der langfristigen Verfügbarkeit und dauerhaften Archivierung der digitalen Edition erfolgt eine strategische Zusammenarbeit mit der Bibliothek des Leibniz-Instituts für Ost- und Südosteuropaforschung (IOS Regensburg, Lambda) sowie der Bayerischen Staatsbibliothek München (BSB München, Osmikon).


### 7. Urheberrechtliche Regelungen


Die Inhalte der digitalen Edition sind unter der Lizenz „CC-BY-NC-ND-4.0 International“ zugänglich.


Die Digitalisate der Reiseaufzeichnungen von Franz Xaver Bronner wurden durch das Staatsarchiv Aargau speziell für diese digitale Edition angefertigt und stehen in der Onlinepräsentation unter der Lizenz „CC0“ zur Verfügung (https://creativecommons.org/publicdomain/zero/1.0/).


Die ODD-Dateien (One Document Does-it-all) werden auf GitHub sowie über Lambda (https://lambda.ios-regensburg.de/) unter der Lizenz „LGPL 3.0“ veröffentlicht.


Die Datensets der Edition wurden als Applikation für die eXist-db entwickelt und stehen ebenfalls auf GitHub unter der Lizenz „LGPL 3.0“ zur Verfügung.


Die Nutzung dieser Onlinepräsentation erfordert den Einsatz von Cookies, die ausschließlich dazu dienen, persönliche Ansichtseinstellungen innerhalb der Edition zu speichern. Dabei werden keinerlei persönliche Informationen erhoben oder gespeichert, und es erfolgt keine Speicherung dieser Daten auf dem Server.


