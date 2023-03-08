---
title: ConnectionParameter Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 10
url: /de/python-net/aspose.cells.externalconnections/connectionparameter/
is_root: false
---
##  ConnectionParameter Klasse
Gibt Eigenschaften zu allen Parametern an, die mit externen Datenverbindungen verwendet werden
Parameter gelten für ODBC- und Webabfragen.



Der Typ ConnectionParameter macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [sql_type](/cells/de/python-net/aspose.cells.externalconnections/connectionparameter/sql_type) | SQL-Datentyp des Parameters. Nur gültig für ODBC-Quellen.|
| [refresh_on_change](/cells/de/python-net/aspose.cells.externalconnections/connectionparameter/refresh_on_change) | Flag, das angibt, ob die Abfrage automatisch aktualisiert werden soll, wenn der Inhalt von a<br/> Zelle, die die Parameterwertänderungen bereitstellt. Wenn wahr, werden externe Daten aktualisiert<br/> Verwendung des neuen Parameterwerts bei jeder Änderung. Wenn falsch, dann externe Daten<br/> wird nur aktualisiert, wenn es vom Benutzer angefordert wird, oder ein anderes Ereignis löst eine Aktualisierung aus (z. B. Arbeitsmappe geöffnet).|
| [prompt](/cells/de/python-net/aspose.cells.externalconnections/connectionparameter/prompt) | Eingabeaufforderungszeichenfolge für den Parameter. Wird dem Tabellenkalkulationsbenutzer zusammen mit der Eingabe-UI angezeigt<br/> um den Parameterwert zu sammeln, bevor die externen Daten aktualisiert werden. Wird nur verwendet, wenn<br/> Parametertyp = Eingabeaufforderung.|
| [type](/cells/de/python-net/aspose.cells.externalconnections/connectionparameter/type) | Typ des verwendeten Parameters.<br/>Wenn parameterType=value, dann der Wert aus boolean, double, integer,<br/> oder string verwendet werden. In diesem Fall wird erwartet, dass nur einer von<br/> {boolean, double, integer oder string} wird angegeben.|
| [name](/cells/de/python-net/aspose.cells.externalconnections/connectionparameter/name) | Der Name des Parameters.|
| [cell_reference](/cells/de/python-net/aspose.cells.externalconnections/connectionparameter/cell_reference) | Cell Verweis, der angibt, welcher Zellenwert für den Abfrageparameter verwendet werden soll. Wird nur verwendet, wenn parameterType cell ist.|
| [value](/cells/de/python-net/aspose.cells.externalconnections/connectionparameter/value) |Nicht ganzzahliger numerischer Wert, ganzzahliger Wert, Zeichenfolgenwert oder boolescher Wert<br/> als Abfrageparameter verwenden. Wird nur verwendet, wenn parameterType gleich value ist.|



###  Siehe auch
* Modul [aspose.cells.externalconnections](..)
