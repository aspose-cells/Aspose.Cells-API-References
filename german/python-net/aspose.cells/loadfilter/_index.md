---
title: LoadFilter Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 1010
url: /de/python-net/aspose.cells/loadfilter/
is_root: false
---
##  LoadFilter Klasse
Stellt den Filter dar, der Optionen zum Laden von Daten bereitstellt, wenn eine Arbeitsmappe aus einer Vorlage geladen wird.



Der Typ LoadFilter macht die folgenden Member verfügbar:

###  Konstrukteure
| Konstrukteur| Beschreibung|
| :- | :- |
| [LoadFilter()](/cells/de/python-net/aspose.cells/loadfilter/__init__/#) | Erstellt einen LoadFilter mit Standardfilteroptionen LoadDataFilterOptions.All.|
| [LoadFilter(opts)](/cells/de/python-net/aspose.cells/loadfilter/__init__/#LoadDataFilterOptions) | Erstellt einen LoadFilter mit gegebenen Filteroptionen.|


###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [load_data_filter_options](/cells/de/python-net/aspose.cells/loadfilter/load_data_filter_options) | Die Filteroptionen geben an, welche Daten geladen werden sollen.|
| [sheets_in_loading_order](/cells/de/python-net/aspose.cells/loadfilter/sheets_in_loading_order) | Gibt die Blätter (Indizes) und die Reihenfolge an, die geladen werden sollen.<br/>Der Standardwert ist null, was bedeutet, dass alle Blätter in der Standardreihenfolge in die Vorlagendatei geladen werden.<br/> Wenn nicht null und der Index eines Blatts nicht im zurückgegebenen Array enthalten ist, wird das Blatt nicht geladen.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [start_sheet(sheet)](/cells/de/python-net/aspose.cells/loadfilter/start_sheet/#Worksheet) | Bereitet Filteroptionen vor dem Laden eines bestimmten Arbeitsblatts vor.<br/>Die Implementierung von LoadFilter durch den Benutzer kann die LoadDataFilterOptions hier ändern<br/> um anzugeben, wie Daten für dieses Arbeitsblatt geladen werden.|



###  Bemerkungen

Der Benutzer kann die Filteroptionen angeben oder eigene LoadFilter implementieren, um anzugeben, wie Daten geladen werden.

###  Siehe auch
* Modul [aspose.cells](..)
