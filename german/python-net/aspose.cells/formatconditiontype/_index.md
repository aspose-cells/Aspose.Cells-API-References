---
title: FormatConditionType Aufzählung
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 2100
url: /de/python-net/aspose.cells/formatconditiontype/
is_root: false
---
##  FormatConditionType Aufzählung
Regeltyp für bedingtes Format.



Der Typ FormatConditionType macht die folgenden Member verfügbar:

###  Felder
| Feld| Beschreibung|
| :- | :- |
| CELL_VALUE | Diese bedingte Formatierungsregel vergleicht einen Zellenwert<br/> zu einem mit einer Formel berechneten Ergebnis unter Verwendung eines Operators.|
| EXPRESSION | Diese Regel zur bedingten Formatierung enthält eine Formel bis<br/>auswerten. Wenn das Formelergebnis wahr ist, ist die Zelle wahr<br/> hervorgehoben.|
| COLOR_SCALE | Diese bedingte Formatierungsregel erstellt eine abgestufte<br/> Farbskala auf den Zellen.|
| DATA_BAR | Diese bedingte Formatierungsregel zeigt ein abgestuftes an<br/> Datenleiste im Bereich der Zellen.|
| ICON_SET |Diese bedingte Formatierungsregel wendet Symbole auf Zellen an<br/> nach ihren Werten.|
| TOP10 | Diese Regel zur bedingten Formatierung hebt Zellen hervor, deren<br/>Werte fallen in die obere N- oder untere N-Klammer, as<br/> angegeben.|
| UNIQUE_VALUES | Diese Regel zur bedingten Formatierung hebt eindeutig hervor<br/> Werte im Bereich.|
| DUPLICATE_VALUES | Diese Regel zur bedingten Formatierung hebt Duplikate hervor<br/> Werte.|
| CONTAINS_TEXT | Diese Regel zur bedingten Formatierung hebt Zellen hervor<br/>gegebenen Text enthalten. Entspricht der Verwendung von SEARCH()<br/>Blattfunktion, um festzustellen, ob die Zelle enthält<br/> der Text.|
| NOT_CONTAINS_TEXT | Diese Regel zur bedingten Formatierung hebt Zellen hervor, die<br/>keinen vorgegebenen Text enthalten. Entspricht der Verwendung von SEARCH()<br/>Blattfunktion, um festzustellen, ob die Zelle enthält<br/> den Text oder nicht.|
| BEGINS_WITH | Diese Regel zur bedingten Formatierung hebt Zellen in hervor<br/>Bereich, die mit dem angegebenen Text beginnen. Gleichwertig<br/> Verwenden der Blattfunktion LEFT() und Vergleichen von Werten.|
| ENDS_WITH | Diese Regel zur bedingten Formatierung hebt Zellenenden hervor<br/>mit vorgegebenem Text. Entspricht der Verwendung des Blatts RIGHT()<br/> Funktion und Vergleichswerte.|
| CONTAINS_BLANKS | Diese Regel zur bedingten Formatierung hebt Zellen hervor, die<br/>sind komplett leer. Entspricht der Verwendung von LEN(TRIM()).<br/>Das heißt, wenn die Zelle nur Zeichen enthält<br/>die TRIM() entfernen würde, dann wird es als leer betrachtet.<br/> Eine leere Zelle gilt ebenfalls als leer.|
| NOT_CONTAINS_BLANKS | Diese Regel zur bedingten Formatierung hebt Zellen hervor, die<br/>sind nicht leer. Entspricht der Verwendung von LEN(TRIM()). Das<br/>bedeutet, dass, wenn die Zelle nur Zeichen enthält, die<br/>TRIM() entfernen würde, dann wird es als leer betrachtet. Ein<br/> Eine leere Zelle wird ebenfalls als leer betrachtet.|
| CONTAINS_ERRORS | Diese bedingte Formatierungsregel hebt Zellen mit hervor<br/>Formelfehler. Entspricht der Verwendung des Blatts ISERROR()<br/> Funktion, um festzustellen, ob ein Formelfehler vorliegt.|
| NOT_CONTAINS_ERRORS | Diese Regel zur bedingten Formatierung hebt Zellen hervor<br/>ohne Formelfehler. Entspricht der Verwendung von ISERROR()<br/> Sheet-Funktion, um festzustellen, ob ein Formelfehler vorliegt.|
| TIME_PERIOD | Diese Regel zur bedingten Formatierung hebt Zellen hervor<br/>Datumsangaben im angegebenen Zeitraum enthalten. Der<br/>Der zugrunde liegende Wert der Zelle wird ausgewertet, daher der<br/>Zelle muss nicht als Datum formatiert werden<br/>ausgewertet. Zum Beispiel mit einer Zelle, die die enthält<br/>Wert 38913 Das bedingte Format soll angewendet werden, wenn<br/> die Regel erfordert einen Wert vom 14.7.2006.|
| ABOVE_AVERAGE | Diese Regel zur bedingten Formatierung hebt Zellen hervor, die<br/>liegen über oder unter dem Durchschnitt für alle Werte in der<br/> Bereich.|



###  Siehe auch
* Modul [aspose.cells](..)
