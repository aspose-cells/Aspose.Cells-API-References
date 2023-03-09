---
title: HtmlLoadOptions Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 770
url: /de/python-net/aspose.cells/htmlloadoptions/
is_root: false
---
##  HtmlLoadOptions Klasse
Repräsentiert Optionen beim Importieren einer HTML-Datei.



**Nachlass:** [HtmlLoadOptions](/cells/python-net/aspose.cells/htmlloadoptions) → 
[AbstractTextLoadOptions](/cells/python-net/aspose.cells/abstracttextloadoptions) → 
[LoadOptions](/cells/de/python-net/aspose.cells/loadoptions)



Der Typ HtmlLoadOptions macht die folgenden Member verfügbar:

###  Konstrukteure
| Konstrukteur| Beschreibung|
| :- | :- |
| [HtmlLoadOptions()](/cells/de/python-net/aspose.cells/htmlloadoptions/__init__/#) | Erstellt eine Option zum Laden der Datei.|
| [HtmlLoadOptions(load_format)](/cells/de/python-net/aspose.cells/htmlloadoptions/__init__/#LoadFormat) | Erstellt eine Option zum Laden der Datei.|


###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [load_format](/cells/de/python-net/aspose.cells/htmlloadoptions/load_format) | Ruft das Ladeformat ab.|
| [password](/cells/de/python-net/aspose.cells/htmlloadoptions/password) | Ruft das Kennwort der Arbeitsmappe ab und legt es fest.|
| [parsing_formula_on_open](/cells/de/python-net/aspose.cells/htmlloadoptions/parsing_formula_on_open) | Gibt an, ob die Formel beim Lesen der Datei analysiert wird.|
| [parsing_pivot_cached_records](/cells/de/python-net/aspose.cells/htmlloadoptions/parsing_pivot_cached_records) | Gibt an, ob beim Laden der Datei zwischengespeicherte Pivot-Datensätze analysiert werden.<br/> Der Standardwert ist falsch.|
| [language_code](/cells/de/python-net/aspose.cells/htmlloadoptions/language_code) | Ruft die Sprache der Benutzeroberfläche der Workbook-Version basierend auf dem CountryCode ab, der die Datei gespeichert hat, oder legt diese fest.|
| [region](/cells/de/python-net/aspose.cells/htmlloadoptions/region) | Ruft die regionalen Systemeinstellungen basierend auf CountryCode zum Zeitpunkt des Ladens der Datei ab oder legt diese fest.|
| [default_style_settings](/cells/de/python-net/aspose.cells/htmlloadoptions/default_style_settings) | Ruft die Standardstileinstellungen zum Initialisieren von Stilen der Arbeitsmappe ab|
| [standard_font](/cells/de/python-net/aspose.cells/htmlloadoptions/standard_font) | Legt den standardmäßigen Standardschriftnamen fest|
| [standard_font_size](/cells/de/python-net/aspose.cells/htmlloadoptions/standard_font_size) | Legt die standardmäßige Standardschriftgröße fest.|
| [interrupt_monitor](/cells/de/python-net/aspose.cells/htmlloadoptions/interrupt_monitor) | Ruft den Interrupt-Monitor ab und setzt ihn.|
| [ignore_not_printed](/cells/de/python-net/aspose.cells/htmlloadoptions/ignore_not_printed) | Ignorieren Sie die nicht gedruckten Daten, wenn Sie die Datei direkt drucken|
| [check_data_valid](/cells/de/python-net/aspose.cells/htmlloadoptions/check_data_valid) |Prüfen Sie, ob die Daten in der Vorlagendatei gültig sind.|
| [check_excel_restriction](/cells/de/python-net/aspose.cells/htmlloadoptions/check_excel_restriction) | Ob die Einschränkung der Excel-Datei überprüft wird, wenn der Benutzer zellenbezogene Objekte ändert.<br/>Beispielsweise erlaubt Excel keine Eingabe von Zeichenfolgenwerten, die länger als 32 KB sind.<br/>Wenn Sie einen Wert eingeben, der länger als 32 KB ist, wie z. B. Cell.PutValue(string), erhalten Sie eine Ausnahme, wenn diese Eigenschaft wahr ist.<br/>Wenn diese Eigenschaft "false" ist, akzeptieren wir Ihren Eingabe-String-Wert als Wert der Zelle, damit dies später möglich ist<br/>bei anderen Dateiformaten wie CSV können Sie den kompletten Stringwert ausgeben.<br/>Wenn Sie jedoch einen solchen Wert festgelegt haben, der für das Excel-Dateiformat ungültig ist,<br/> Sie sollten die Arbeitsmappe später nicht als Excel-Dateiformat speichern.|
| [keep_unparsed_data](/cells/de/python-net/aspose.cells/htmlloadoptions/keep_unparsed_data) | Ob die ungeparsten Daten für die Arbeitsmappe im Arbeitsspeicher bleiben, wenn sie aus der Vorlagendatei geladen wird. Der Standardwert ist „true“.|
| [load_filter](/cells/de/python-net/aspose.cells/htmlloadoptions/load_filter) | Der Filter, der angibt, wie Daten geladen werden.|
| [light_cells_data_handler](/cells/de/python-net/aspose.cells/htmlloadoptions/light_cells_data_handler) | Der Datenhandler zum Verarbeiten von Zellendaten beim Lesen der Vorlagendatei.|
| [memory_setting](/cells/de/python-net/aspose.cells/htmlloadoptions/memory_setting) | Ruft die Speichernutzungsoptionen ab oder legt diese fest.|
| [warning_callback](/cells/de/python-net/aspose.cells/htmlloadoptions/warning_callback) | Ruft Warnungsrückrufe ab oder legt sie fest.|
| [auto_fitter_options](/cells/de/python-net/aspose.cells/htmlloadoptions/auto_fitter_options) | Ruft die Autofitter-Optionen ab und legt sie fest|
| [auto_filter](/cells/de/python-net/aspose.cells/htmlloadoptions/auto_filter) | Gibt an, ob die Daten beim Laden der Dateien automatisch gefiltert werden.|
| [font_configs](/cells/de/python-net/aspose.cells/htmlloadoptions/font_configs) | Ruft individuelle Schriftartkonfigurationen ab und legt sie fest.<br/> Funktioniert nur für die [Workbook](/cells/de/python-net/aspose.cells/workbook), die diese [LoadOptions](/cells/de/python-net/aspose.cells/loadoptions) zum Laden verwendet.|
| [encoding](/cells/de/python-net/aspose.cells/htmlloadoptions/encoding) | Ruft die Standardcodierung ab und legt sie fest.|
| [load_style_strategy](/cells/de/python-net/aspose.cells/htmlloadoptions/load_style_strategy) |Gibt die Strategie zum Anwenden des Stils für geparste Werte beim Konvertieren von Zeichenfolgenwerten in Zahlen oder Datumsangaben an.|
| [convert_numeric_data](/cells/de/python-net/aspose.cells/htmlloadoptions/convert_numeric_data) | Ruft einen Wert ab, der angibt, ob die Zeichenfolge in der Textdatei in numerische Daten konvertiert wird, oder legt diesen fest.|
| [convert_date_time_data](/cells/de/python-net/aspose.cells/htmlloadoptions/convert_date_time_data) | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob die Zeichenfolge in der Textdatei in Datumsdaten konvertiert wird.|
| [keep_precision](/cells/de/python-net/aspose.cells/htmlloadoptions/keep_precision) | Gibt an, ob ein Zeichenfolgenwert bei einer Länge von 15 nicht analysiert wird.|
| [attached_files_directory](/cells/de/python-net/aspose.cells/htmlloadoptions/attached_files_directory) | Das Verzeichnis, in dem die angehängten Dateien gespeichert werden.|
| [load_formulas](/cells/de/python-net/aspose.cells/htmlloadoptions/load_formulas) | Gibt an, ob Formeln importiert werden, wenn die ursprüngliche HTML-Datei Formeln enthält|
| [support_div_tag](/cells/de/python-net/aspose.cells/htmlloadoptions/support_div_tag) | Gibt an, ob das Layout von unterstützt wird<div> Tag, wenn die HTML-Datei enthält<div> Stichworte.|
| [delete_redundant_spaces](/cells/de/python-net/aspose.cells/htmlloadoptions/delete_redundant_spaces) | Gibt an, ob überflüssige Leerzeichen gelöscht werden sollen, wenn der Text Zeilen mit umbricht<br> Der Standardwert ist „false“.|
| [auto_fit_cols_and_rows](/cells/de/python-net/aspose.cells/htmlloadoptions/auto_fit_cols_and_rows) | Gibt an, ob Spalten und Zeilen automatisch angepasst werden.|
| [convert_formulas_data](/cells/de/python-net/aspose.cells/htmlloadoptions/convert_formulas_data) | Wenn wahr, Zeichenfolge in Formel konvertieren, wenn der Zeichenfolgenwert mit dem Zeichen „=“ beginnt, ist der Standardwert falsch.|
| [stream_provider](/cells/de/python-net/aspose.cells/htmlloadoptions/stream_provider) | Ruft die StreamProviderImportHtmlFile zum Importieren von Objekten ab oder legt diese fest.|
| [prog_id](/cells/de/python-net/aspose.cells/htmlloadoptions/prog_id) | Ruft die Programm-ID zum Erstellen der Datei ab.<br/> Nur für MHT-Dateien.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [set_paper_size(type)](/cells/de/python-net/aspose.cells/htmlloadoptions/set_paper_size/#PaperSizeType) | Legt das Standarddruckpapierformat aus der Standarddruckereinstellung fest.|



###  Siehe auch
* Modul [aspose.cells](..)
* Klasse [AbstractTextLoadOptions](/cells/de/python-net/aspose.cells/abstracttextloadoptions)
* Klasse [HtmlLoadOptions](/cells/de/python-net/aspose.cells/htmlloadoptions)
* Klasse [LoadOptions](/cells/de/python-net/aspose.cells/loadoptions)
* Klasse [Workbook](/cells/de/python-net/aspose.cells/workbook)
