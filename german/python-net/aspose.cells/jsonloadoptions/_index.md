---
title: JsonLoadOptions Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 960
url: /de/python-net/aspose.cells/jsonloadoptions/
is_root: false
---
##  JsonLoadOptions Klasse
Stellt die Optionen zum Laden von JSON-Dateien dar



**Nachlass:** [JsonLoadOptions](/cells/python-net/aspose.cells/jsonloadoptions) → 
[LoadOptions](/cells/de/python-net/aspose.cells/loadoptions)



Der Typ JsonLoadOptions macht die folgenden Member verfügbar:

###  Konstrukteure
| Konstrukteur| Beschreibung|
| :- | :- |
| [JsonLoadOptions()](/cells/de/python-net/aspose.cells/jsonloadoptions/__init__/#) | Erstellt Optionen zum Laden der Datei.|


###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [load_format](/cells/de/python-net/aspose.cells/jsonloadoptions/load_format) | Ruft das Ladeformat ab.|
| [password](/cells/de/python-net/aspose.cells/jsonloadoptions/password) | Ruft das Kennwort der Arbeitsmappe ab und legt es fest.|
| [parsing_formula_on_open](/cells/de/python-net/aspose.cells/jsonloadoptions/parsing_formula_on_open) | Gibt an, ob die Formel beim Lesen der Datei analysiert wird.|
| [parsing_pivot_cached_records](/cells/de/python-net/aspose.cells/jsonloadoptions/parsing_pivot_cached_records) | Gibt an, ob beim Laden der Datei zwischengespeicherte Pivot-Datensätze analysiert werden.<br/> Der Standardwert ist falsch.|
| [language_code](/cells/de/python-net/aspose.cells/jsonloadoptions/language_code) | Ruft die Sprache der Benutzeroberfläche der Workbook-Version basierend auf dem CountryCode ab, der die Datei gespeichert hat, oder legt diese fest.|
| [region](/cells/de/python-net/aspose.cells/jsonloadoptions/region) | Ruft die regionalen Systemeinstellungen basierend auf CountryCode zum Zeitpunkt des Ladens der Datei ab oder legt diese fest.|
| [default_style_settings](/cells/de/python-net/aspose.cells/jsonloadoptions/default_style_settings) | Ruft die Standardstileinstellungen zum Initialisieren von Stilen der Arbeitsmappe ab|
| [standard_font](/cells/de/python-net/aspose.cells/jsonloadoptions/standard_font) | Legt den standardmäßigen Standardschriftnamen fest|
| [standard_font_size](/cells/de/python-net/aspose.cells/jsonloadoptions/standard_font_size) | Legt die standardmäßige Standardschriftgröße fest.|
| [interrupt_monitor](/cells/de/python-net/aspose.cells/jsonloadoptions/interrupt_monitor) | Ruft den Interrupt-Monitor ab und setzt ihn.|
| [ignore_not_printed](/cells/de/python-net/aspose.cells/jsonloadoptions/ignore_not_printed) | Ignorieren Sie die nicht gedruckten Daten, wenn Sie die Datei direkt drucken|
| [check_data_valid](/cells/de/python-net/aspose.cells/jsonloadoptions/check_data_valid) | Prüfen Sie, ob die Daten in der Vorlagendatei gültig sind.|
| [check_excel_restriction](/cells/de/python-net/aspose.cells/jsonloadoptions/check_excel_restriction) | Ob die Einschränkung der Excel-Datei überprüft wird, wenn der Benutzer zellenbezogene Objekte ändert.<br/>Beispielsweise erlaubt Excel keine Eingabe von Zeichenfolgenwerten, die länger als 32 KB sind.<br/>Wenn Sie einen Wert eingeben, der länger als 32 KB ist, wie z. B. Cell.PutValue(string), erhalten Sie eine Ausnahme, wenn diese Eigenschaft wahr ist.<br/>Wenn diese Eigenschaft "false" ist, akzeptieren wir Ihren Eingabe-String-Wert als Wert der Zelle, damit dies später möglich ist<br/>bei anderen Dateiformaten wie CSV können Sie den kompletten Stringwert ausgeben.<br/>Wenn Sie jedoch einen solchen Wert festgelegt haben, der für das Excel-Dateiformat ungültig ist,<br/> Sie sollten die Arbeitsmappe später nicht als Excel-Dateiformat speichern. Andernfalls kann es zu unerwarteten Fehlern in der generierten Excel-Datei kommen.|
| [keep_unparsed_data](/cells/de/python-net/aspose.cells/jsonloadoptions/keep_unparsed_data) |Ob die ungeparsten Daten für die Arbeitsmappe im Arbeitsspeicher bleiben, wenn sie aus der Vorlagendatei geladen wird. Standard ist wahr.|
| [load_filter](/cells/de/python-net/aspose.cells/jsonloadoptions/load_filter) | Der Filter, der angibt, wie Daten geladen werden.|
| [light_cells_data_handler](/cells/de/python-net/aspose.cells/jsonloadoptions/light_cells_data_handler) | Der Datenhandler zum Verarbeiten von Zellendaten beim Lesen der Vorlagendatei.|
| [memory_setting](/cells/de/python-net/aspose.cells/jsonloadoptions/memory_setting) | Ruft die Speichernutzungsoptionen ab oder legt diese fest.|
| [warning_callback](/cells/de/python-net/aspose.cells/jsonloadoptions/warning_callback) | Ruft einen Warnungsrückruf ab oder legt ihn fest.|
| [auto_fitter_options](/cells/de/python-net/aspose.cells/jsonloadoptions/auto_fitter_options) | Ruft die Autofitter-Optionen ab und legt sie fest|
| [auto_filter](/cells/de/python-net/aspose.cells/jsonloadoptions/auto_filter) | Gibt an, ob die Daten beim Laden der Dateien automatisch gefiltert werden.|
| [font_configs](/cells/de/python-net/aspose.cells/jsonloadoptions/font_configs) | Ruft individuelle Schriftartkonfigurationen ab und legt sie fest.<br/> Funktioniert nur für die [Workbook](/cells/de/python-net/aspose.cells/workbook), die diese [LoadOptions](/cells/de/python-net/aspose.cells/loadoptions) zum Laden verwendet.|
| [start_cell](/cells/de/python-net/aspose.cells/jsonloadoptions/start_cell) | Ruft die Startzelle ab und legt sie fest.|
| [layout_options](/cells/de/python-net/aspose.cells/jsonloadoptions/layout_options) | Die Importoptionen von json.|
| [multiple_worksheets](/cells/de/python-net/aspose.cells/jsonloadoptions/multiple_worksheets) | Gibt an, ob jedes Attribut des JsonObject-Objekts als ein Arbeitsblatt importiert wird, wenn alle untergeordneten Knoten Arrayknoten sind.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [set_paper_size(type)](/cells/de/python-net/aspose.cells/jsonloadoptions/set_paper_size/#PaperSizeType) | Legt das Standarddruckpapierformat aus der Standarddruckereinstellung fest.|



###  Siehe auch
* Modul [aspose.cells](..)
* Klasse [JsonLoadOptions](/cells/de/python-net/aspose.cells/jsonloadoptions)
* Klasse [LoadOptions](/cells/de/python-net/aspose.cells/loadoptions)
* Klasse [Workbook](/cells/de/python-net/aspose.cells/workbook)
