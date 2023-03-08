---
title: TxtSaveOptions Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 1520
url: /de/python-net/aspose.cells/txtsaveoptions/
is_root: false
---
##  TxtSaveOptions Klasse
Stellt die Speicheroptionen für CSV/tabulatorgetrenntes/anderes Textformat dar.



**Nachlass:** [TxtSaveOptions](/cells/python-net/aspose.cells/txtsaveoptions) → 
[SaveOptions](/cells/de/python-net/aspose.cells/saveoptions)



Der Typ TxtSaveOptions macht die folgenden Member verfügbar:

###  Konstrukteure
| Konstrukteur| Beschreibung|
| :- | :- |
| [TxtSaveOptions()](/cells/de/python-net/aspose.cells/txtsaveoptions/__init__/#) | Erstellt Optionen zum Speichern von Textdateien.|
| [TxtSaveOptions(format)](/cells/de/python-net/aspose.cells/txtsaveoptions/__init__/#SaveFormat) | Erstellt Optionen zum Speichern von Textdateien.|


###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [save_format](/cells/de/python-net/aspose.cells/txtsaveoptions/save_format) | Ruft das Sicherungsdateiformat ab.|
| [clear_data](/cells/de/python-net/aspose.cells/txtsaveoptions/clear_data) | Machen Sie die Arbeitsmappe nach dem Speichern der Datei leer.|
| [cached_file_folder](/cells/de/python-net/aspose.cells/txtsaveoptions/cached_file_folder) | Der zwischengespeicherte Dateiordner wird verwendet, um einige große Daten zu speichern.|
| [validate_merged_areas](/cells/de/python-net/aspose.cells/txtsaveoptions/validate_merged_areas) | Gibt an, ob verbundene Zellen vor dem Speichern der Datei validiert werden sollen.|
| [merge_areas](/cells/de/python-net/aspose.cells/txtsaveoptions/merge_areas) | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden sollen.|
| [create_directory](/cells/de/python-net/aspose.cells/txtsaveoptions/create_directory) | Wenn wahr und das Verzeichnis nicht existiert, wird das Verzeichnis automatisch erstellt, bevor die Datei gespeichert wird.|
| [sort_names](/cells/de/python-net/aspose.cells/txtsaveoptions/sort_names) | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden.|
| [sort_external_names](/cells/de/python-net/aspose.cells/txtsaveoptions/sort_external_names) | Gibt an, ob extern definierte Namen vor dem Speichern der Datei sortiert werden.|
| [refresh_chart_cache](/cells/de/python-net/aspose.cells/txtsaveoptions/refresh_chart_cache) |Gibt an, ob Diagramm-Cache-Daten aktualisiert werden|
| [warning_callback](/cells/de/python-net/aspose.cells/txtsaveoptions/warning_callback) | Ruft einen Warnungsrückruf ab oder legt ihn fest.|
| [update_smart_art](/cells/de/python-net/aspose.cells/txtsaveoptions/update_smart_art) | Gibt an, ob die SmartArt-Einstellung aktualisiert wird.<br/> Der Standardwert ist falsch.|
| [separator](/cells/de/python-net/aspose.cells/txtsaveoptions/separator) | Ruft das Zeichentrennzeichen der Textdatei ab und legt es fest.|
| [separator_string](/cells/de/python-net/aspose.cells/txtsaveoptions/separator_string) | Ruft einen Zeichenfolgenwert als Trennzeichen ab und legt ihn fest.|
| [encoding](/cells/de/python-net/aspose.cells/txtsaveoptions/encoding) | Ruft die Standardcodierung ab und legt sie fest.|
| [always_quoted](/cells/de/python-net/aspose.cells/txtsaveoptions/always_quoted) | Gibt an, ob immer '"' für jedes Feld hinzugefügt wird.<br/>Wenn wahr, werden alle Werte in Anführungszeichen gesetzt;<br/>Wenn falsch, werden die Werte nur bei Bedarf angegeben (z. B.<br/>wenn Werte Sonderzeichen wie '"' , '\n' oder Trennzeichen enthalten).<br/> Standard ist falsch.|
| [quote_type](/cells/de/python-net/aspose.cells/txtsaveoptions/quote_type) | Ruft ab oder legt fest, wie Werte in der exportierten Textdatei zitiert werden.|
| [format_strategy](/cells/de/python-net/aspose.cells/txtsaveoptions/format_strategy) |Ruft die Formatstrategie ab und legt sie fest, wenn der Zellenwert als Zeichenfolge exportiert wird.|
| [light_cells_data_provider](/cells/de/python-net/aspose.cells/txtsaveoptions/light_cells_data_provider) | Der Datenanbieter zum Bereitstellen von Zellendaten zum Speichern von Arbeitsmappen im Light-Modus.|
| [trim_leading_blank_row_and_column](/cells/de/python-net/aspose.cells/txtsaveoptions/trim_leading_blank_row_and_column) | Gibt an, ob führende leere Zeilen und Spalten gekürzt werden sollen, wie es MS Excel tut.<br/> Standard ist wahr.|
| [trim_tailing_blank_cells](/cells/de/python-net/aspose.cells/txtsaveoptions/trim_tailing_blank_cells) |Gibt an, ob nachlaufende leere Zellen in einer Zeile gekürzt werden sollen. Standard ist falsch.|
| [keep_separators_for_blank_row](/cells/de/python-net/aspose.cells/txtsaveoptions/keep_separators_for_blank_row) |Gibt an, ob Trennzeichen für Leerzeilen ausgegeben werden sollen.<br/> Der Standardwert ist „false“, sodass der Inhalt für eine leere Zeile standardmäßig leer ist.|
| [export_area](/cells/de/python-net/aspose.cells/txtsaveoptions/export_area) | Der Bereich der zu exportierenden Zellen.|
| [export_quote_prefix](/cells/de/python-net/aspose.cells/txtsaveoptions/export_quote_prefix) | Gibt an, ob das einfache Anführungszeichen als Teil des Werts einer Zelle exportiert werden soll<br/> wenn [Style.quote_prefix](/cells/de/python-net/aspose.cells/style#quote_prefix) dafür gilt. Standard ist falsch.|
| [export_all_sheets](/cells/de/python-net/aspose.cells/txtsaveoptions/export_all_sheets) | Gibt an, ob alle Blätter in die Textdatei exportiert werden.<br/> Wenn es falsch ist, exportieren Sie nur das aktive Blatt, genau wie MS Excel.|



###  Siehe auch
* Modul [aspose.cells](..)
* Klasse [SaveOptions](/cells/de/python-net/aspose.cells/saveoptions)
* Klasse [TxtSaveOptions](/cells/de/python-net/aspose.cells/txtsaveoptions)
