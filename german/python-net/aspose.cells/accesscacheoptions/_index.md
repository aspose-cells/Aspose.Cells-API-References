---
title: AccessCacheOptions Aufzählung
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 1740
url: /de/python-net/aspose.cells/accesscacheoptions/
is_root: false
---
##  AccessCacheOptions Aufzählung
Cache-Optionen für den Datenzugriff. Kann mit | kombiniert werden Operator für mehrere Optionen zusammen.



Der Typ AccessCacheOptions macht die folgenden Member verfügbar:

###  Felder
| Feld| Beschreibung|
| :- | :- |
| NONE | Kein Cache für jeglichen Datenzugriff.|
| ALL | Wenden Sie alle möglichen Optimierungen für alle Arten von Datenzugriffen in der Arbeitsmappe an.<br/> Alle Einstellungen und Daten sollten während des optimierten Zugriffs nicht verändert werden.|
| POSITION_AND_SIZE | Wenden Sie eine mögliche Optimierung an, um die Position und Größe von Objekten (z. B. Form) zu erhalten.<br/>Die Einstellungen für Zeilenhöhe und Spaltenbreite sollten während des optimierten Zugriffs nicht geändert werden.|
| CELLS_DATA | Wenden Sie eine mögliche Optimierung an, um die Werte der Zellen zu erhalten.<br/>Cells-Daten (Daten und Einstellungen von Cell, Zeile) sollten währenddessen nicht geändert werden<br/>Beim optimierten Zugriff sollten auch keine neuen Cell/Row-Objekte erstellt werden (wie z<br/> von [[indexer]](/cells/python-net/aspose.cells/cells/__getitem__/)).|
| CELL_DISPLAY | Wenden Sie eine mögliche Optimierung an, um anzeigebezogene Ergebnisse zu erhalten<br/>Zellen ([Cell.display_string_value](/cells/de/python-net/aspose.cells/cell#display_string_value), [Cell.get_style()](/cells/de/python-net/aspose.cells/cell/get_style), [Cell.get_display_style()](/cells/de/python-net/aspose.cells/cell/get_display_style) usw.).<br/>Cells Daten- und stilbezogene Objekte (Cell/Zeilen-/Spaltenstile, Spaltenbreite usw.) sollten nicht geändert werden<br/> während des optimierten Zugriffs.|
| GET_FORMULA | Wenden Sie mögliche Optimierungen zum Abrufen von Formeln an.<br/>Alle Daten und Einstellungen, die sich auf den Formelausdruck auswirken können (Name des Arbeitsblatts, Text des Namens,<br/> Tabellenspalte usw.) sollten während des optimierten Zugriffs nicht verändert werden.|
| SET_FORMULA | Wenden Sie mögliche Optimierungen für Einstellungsformeln an.<br/>Alle Daten und Einstellungen, die sich auf den Formelausdruck auswirken können (Name des Arbeitsblatts, Text des Namens,<br/> Tabellenspalte usw.) sollten während des optimierten Zugriffs nicht verändert werden.|
| CALCULATE_FORMULA |Wenden Sie mögliche Optimierungen für die Berechnung von Formeln an.<br/>Cells Daten sollten beim optimierten Zugriff nicht verändert werden, keine neuen Objekte (Cell, Row, etc.)<br/> sollte entweder erstellt werden (z. B. von [[indexer]] (/cells/python-net/aspose.cells/cells/__getitem__/)).|
| CONDITIONAL_FORMATTING | Wenden Sie eine mögliche Optimierung an, um das Formatierungsergebnis bedingter Formatierungen zu erhalten.<br/>Alle Daten und Einstellungen, die das Ergebnis von bedingten Formatierungen beeinflussen können (Einstellungen von<br/> bedingte Formatierungen, abhängige Zellwerte etc.) sollten während des optimierten Zugriffs nicht verändert werden.|
| VALIDATION | Wenden Sie eine mögliche Optimierung an, um das Validierungsergebnis zu erhalten.<br/>Alle Daten und Einstellungen, die das Ergebnis der Validierung beeinflussen können (Einstellungen der Validierung,<br/> abhängige Zellenwerte etc.) sollten während des optimierten Zugriffs nicht verändert werden.|



###  Bemerkungen

Bei einigen Funktionen erfordert der Zugriff auf große Datensätze viele wiederholte und komplizierte Vorgänge
wie Suche, Berechnung usw. und diese Operationen werden viel zusätzliche Zeit in Anspruch nehmen.
Für häufige Situationen bleiben alle abhängigen Daten während des Zugriffs unverändert, sodass einige Caches erstellt und verwendet werden können
verbessert die Zugriffsleistung.
Zu diesem Zweck stellen wir diese API bereit, damit der Benutzer angeben kann, welche Art von Datenzugriff erforderlich ist
durch mögliche Caching-Mechanismen optimiert werden.


Bitte beachten Sie, dass für verschiedene Optionen möglicherweise andere Datensätze "schreibgeschützt" sein müssen.
Und die Leistung des Datenzugriffs hängt von vielen Aspekten ab, der Verwendung des Caching-Mechanismus
garantiert nicht, dass die Leistung verbessert wird. Für manche Situationen
B. der Datensatz, auf den zugegriffen werden soll, klein ist, kann die Verwendung des Caches sogar noch mehr Zeit in Anspruch nehmen, weil
Das Caching selbst erfordert auch eine gewisse zusätzliche Zeit.

###  Siehe auch
* Modul [aspose.cells](..)
