---
title: XmlLoadOptions Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 1690
url: /de/python-net/aspose.cells/xmlloadoptions/
is_root: false
---
##  XmlLoadOptions Klasse
Repräsentiert die Optionen zum Laden von XML.



**Nachlass:** [XmlLoadOptions](/cells/python-net/aspose.cells/xmlloadoptions) → 
[LoadOptions](/cells/de/python-net/aspose.cells/loadoptions)



Der Typ XmlLoadOptions macht die folgenden Member verfügbar:

###  Konstrukteure
| Konstrukteur| Beschreibung|
| :- | :- |
| [XmlLoadOptions()](/cells/de/python-net/aspose.cells/xmlloadoptions/__init__/#) | Stellt die Optionen zum Laden der XML-Datei dar.|
| [XmlLoadOptions(type)](/cells/de/python-net/aspose.cells/xmlloadoptions/__init__/#LoadFormat) | Stellt die Optionen zum Laden der XML-Datei dar.|


###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [load_format](/cells/de/python-net/aspose.cells/xmlloadoptions/load_format) | Ruft das Ladeformat ab.|
| [password](/cells/de/python-net/aspose.cells/xmlloadoptions/password) | Ruft das Kennwort der Arbeitsmappe ab und legt es fest.|
| [parsing_formula_on_open](/cells/de/python-net/aspose.cells/xmlloadoptions/parsing_formula_on_open) | Gibt an, ob die Formel beim Lesen der Datei analysiert wird.|
| [parsing_pivot_cached_records](/cells/de/python-net/aspose.cells/xmlloadoptions/parsing_pivot_cached_records) | Gibt an, ob beim Laden der Datei zwischengespeicherte Pivot-Datensätze analysiert werden.<br/> Der Standardwert ist falsch.|
| [language_code](/cells/de/python-net/aspose.cells/xmlloadoptions/language_code) | Ruft die Sprache der Benutzeroberfläche der Workbook-Version basierend auf dem CountryCode ab, der die Datei gespeichert hat, oder legt diese fest.|
| [region](/cells/de/python-net/aspose.cells/xmlloadoptions/region) | Ruft die regionalen Systemeinstellungen basierend auf CountryCode zum Zeitpunkt des Ladens der Datei ab oder legt diese fest.|
| [default_style_settings](/cells/de/python-net/aspose.cells/xmlloadoptions/default_style_settings) | Ruft die Standardstileinstellungen zum Initialisieren von Stilen der Arbeitsmappe ab|
| [standard_font](/cells/de/python-net/aspose.cells/xmlloadoptions/standard_font) | Legt den standardmäßigen Standardschriftnamen fest|
| [standard_font_size](/cells/de/python-net/aspose.cells/xmlloadoptions/standard_font_size) | Legt die standardmäßige Standardschriftgröße fest.|
| [interrupt_monitor](/cells/de/python-net/aspose.cells/xmlloadoptions/interrupt_monitor) | Ruft den Interrupt-Monitor ab und setzt ihn.|
| [ignore_not_printed](/cells/de/python-net/aspose.cells/xmlloadoptions/ignore_not_printed) | Ignorieren Sie die nicht gedruckten Daten, wenn Sie die Datei direkt drucken|
| [check_data_valid](/cells/de/python-net/aspose.cells/xmlloadoptions/check_data_valid) |Prüfen Sie, ob die Daten in der Vorlagendatei gültig sind.|
| [check_excel_restriction](/cells/de/python-net/aspose.cells/xmlloadoptions/check_excel_restriction) | Ob die Einschränkung der Excel-Datei überprüft wird, wenn der Benutzer zellenbezogene Objekte ändert.<br/>Beispielsweise erlaubt Excel keine Eingabe von Zeichenfolgenwerten, die länger als 32 KB sind.<br/>Wenn Sie einen Wert eingeben, der länger als 32 KB ist, wie z. B. Cell.PutValue(string), erhalten Sie eine Ausnahme, wenn diese Eigenschaft wahr ist.<br/>Wenn diese Eigenschaft "false" ist, akzeptieren wir Ihren Eingabe-String-Wert als Wert der Zelle, damit dies später möglich ist<br/>bei anderen Dateiformaten wie CSV können Sie den kompletten Stringwert ausgeben.<br/>Wenn Sie jedoch einen solchen Wert festgelegt haben, der für das Excel-Dateiformat ungültig ist,<br/> Sie sollten die Arbeitsmappe später nicht als Excel-Dateiformat speichern.|
| [keep_unparsed_data](/cells/de/python-net/aspose.cells/xmlloadoptions/keep_unparsed_data) | Ob die ungeparsten Daten für die Arbeitsmappe im Arbeitsspeicher bleiben, wenn sie aus der Vorlagendatei geladen wird. Der Standardwert ist „true“.|
| [load_filter](/cells/de/python-net/aspose.cells/xmlloadoptions/load_filter) | Der Filter, der angibt, wie Daten geladen werden.|
| [light_cells_data_handler](/cells/de/python-net/aspose.cells/xmlloadoptions/light_cells_data_handler) | Der Datenhandler zum Verarbeiten von Zellendaten beim Lesen der Vorlagendatei.|
| [memory_setting](/cells/de/python-net/aspose.cells/xmlloadoptions/memory_setting) | Ruft die Speichernutzungsoptionen ab oder legt diese fest.|
| [warning_callback](/cells/de/python-net/aspose.cells/xmlloadoptions/warning_callback) | Ruft Warnungsrückrufe ab oder legt sie fest.|
| [auto_fitter_options](/cells/de/python-net/aspose.cells/xmlloadoptions/auto_fitter_options) | Ruft die Autofitter-Optionen ab und legt sie fest|
| [auto_filter](/cells/de/python-net/aspose.cells/xmlloadoptions/auto_filter) | Gibt an, ob die Daten beim Laden der Dateien automatisch gefiltert werden.|
| [font_configs](/cells/de/python-net/aspose.cells/xmlloadoptions/font_configs) | Ruft individuelle Schriftartkonfigurationen ab und legt sie fest.<br/> Funktioniert nur für die [Workbook](/cells/de/python-net/aspose.cells/workbook), die diese [LoadOptions](/cells/de/python-net/aspose.cells/loadoptions) zum Laden verwendet.|
| [start_cell](/cells/de/python-net/aspose.cells/xmlloadoptions/start_cell) | Ruft die Startzelle ab und legt sie fest.|
| [is_xml_map](/cells/de/python-net/aspose.cells/xmlloadoptions/is_xml_map) |Gibt an, ob XML zu Excel zugeordnet wird.<br/> Der Standardwert ist falsch.|
| [contains_multiple_worksheets](/cells/de/python-net/aspose.cells/xmlloadoptions/contains_multiple_worksheets) | Gibt an, ob XML als mehrere Arbeitsblätter importiert werden.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [set_paper_size(type)](/cells/de/python-net/aspose.cells/xmlloadoptions/set_paper_size/#PaperSizeType) | Legt das Standarddruckpapierformat aus der Standarddruckereinstellung fest.|



###  Siehe auch
* Modul [aspose.cells](..)
* Klasse [LoadOptions](/cells/de/python-net/aspose.cells/loadoptions)
* Klasse [Workbook](/cells/de/python-net/aspose.cells/workbook)
* Klasse [XmlLoadOptions](/cells/de/python-net/aspose.cells/xmlloadoptions)
