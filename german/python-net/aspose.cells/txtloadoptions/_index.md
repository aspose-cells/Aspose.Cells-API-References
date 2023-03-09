---
title: TxtLoadOptions Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 1510
url: /de/python-net/aspose.cells/txtloadoptions/
is_root: false
---
##  TxtLoadOptions Klasse
Repräsentiert die Optionen zum Laden von Textdateien.



**Nachlass:** [TxtLoadOptions](/cells/python-net/aspose.cells/txtloadoptions) → 
[AbstractTextLoadOptions](/cells/python-net/aspose.cells/abstracttextloadoptions) → 
[LoadOptions](/cells/de/python-net/aspose.cells/loadoptions)



Der Typ TxtLoadOptions macht die folgenden Member verfügbar:

###  Konstrukteure
| Konstrukteur| Beschreibung|
| :- | :- |
| [TxtLoadOptions()](/cells/de/python-net/aspose.cells/txtloadoptions/__init__/#) | Erstellt die Optionen zum Laden von Textdateien.|
| [TxtLoadOptions(load_format)](/cells/de/python-net/aspose.cells/txtloadoptions/__init__/#LoadFormat) | Erstellt die Optionen zum Laden von Textdateien.|


###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [load_format](/cells/de/python-net/aspose.cells/txtloadoptions/load_format) | Ruft das Ladeformat ab.|
| [password](/cells/de/python-net/aspose.cells/txtloadoptions/password) | Ruft das Kennwort der Arbeitsmappe ab und legt es fest.|
| [parsing_formula_on_open](/cells/de/python-net/aspose.cells/txtloadoptions/parsing_formula_on_open) | Gibt an, ob die Formel beim Lesen der Datei analysiert wird.|
| [parsing_pivot_cached_records](/cells/de/python-net/aspose.cells/txtloadoptions/parsing_pivot_cached_records) | Gibt an, ob beim Laden der Datei zwischengespeicherte Pivot-Datensätze analysiert werden.<br/> Der Standardwert ist falsch.|
| [language_code](/cells/de/python-net/aspose.cells/txtloadoptions/language_code) | Ruft die Sprache der Benutzeroberfläche der Workbook-Version basierend auf dem CountryCode ab, der die Datei gespeichert hat, oder legt diese fest.|
| [region](/cells/de/python-net/aspose.cells/txtloadoptions/region) | Ruft die regionalen Systemeinstellungen basierend auf CountryCode zum Zeitpunkt des Ladens der Datei ab oder legt diese fest.|
| [default_style_settings](/cells/de/python-net/aspose.cells/txtloadoptions/default_style_settings) | Ruft die Standardstileinstellungen zum Initialisieren von Stilen der Arbeitsmappe ab|
| [standard_font](/cells/de/python-net/aspose.cells/txtloadoptions/standard_font) | Legt den standardmäßigen Standardschriftnamen fest|
| [standard_font_size](/cells/de/python-net/aspose.cells/txtloadoptions/standard_font_size) | Legt die standardmäßige Standardschriftgröße fest.|
| [interrupt_monitor](/cells/de/python-net/aspose.cells/txtloadoptions/interrupt_monitor) | Ruft den Interrupt-Monitor ab und setzt ihn.|
| [ignore_not_printed](/cells/de/python-net/aspose.cells/txtloadoptions/ignore_not_printed) | Ignorieren Sie die nicht gedruckten Daten, wenn Sie die Datei direkt drucken|
| [check_data_valid](/cells/de/python-net/aspose.cells/txtloadoptions/check_data_valid) |Prüfen Sie, ob die Daten in der Vorlagendatei gültig sind.|
| [check_excel_restriction](/cells/de/python-net/aspose.cells/txtloadoptions/check_excel_restriction) | Ob die Einschränkung der Excel-Datei überprüft wird, wenn der Benutzer zellenbezogene Objekte ändert.<br/>Beispielsweise erlaubt Excel keine Eingabe von Zeichenfolgenwerten, die länger als 32 KB sind.<br/>Wenn Sie einen Wert eingeben, der länger als 32 KB ist, wie z. B. Cell.PutValue(string), erhalten Sie eine Ausnahme, wenn diese Eigenschaft wahr ist.<br/>Wenn diese Eigenschaft "false" ist, akzeptieren wir Ihren Eingabe-String-Wert als Wert der Zelle, damit dies später möglich ist<br/>bei anderen Dateiformaten wie CSV können Sie den kompletten Stringwert ausgeben.<br/>Wenn Sie jedoch einen solchen Wert festgelegt haben, der für das Excel-Dateiformat ungültig ist,<br/> Sie sollten die Arbeitsmappe später nicht als Excel-Dateiformat speichern.|
| [keep_unparsed_data](/cells/de/python-net/aspose.cells/txtloadoptions/keep_unparsed_data) | Ob die ungeparsten Daten für die Arbeitsmappe im Arbeitsspeicher bleiben, wenn sie aus der Vorlagendatei geladen wird. Der Standardwert ist „true“.|
| [load_filter](/cells/de/python-net/aspose.cells/txtloadoptions/load_filter) | Der Filter, der angibt, wie Daten geladen werden.|
| [light_cells_data_handler](/cells/de/python-net/aspose.cells/txtloadoptions/light_cells_data_handler) | Der Datenhandler zum Verarbeiten von Zellendaten beim Lesen der Vorlagendatei.|
| [memory_setting](/cells/de/python-net/aspose.cells/txtloadoptions/memory_setting) | Ruft die Speichernutzungsoptionen ab oder legt diese fest.|
| [warning_callback](/cells/de/python-net/aspose.cells/txtloadoptions/warning_callback) | Ruft Warnungsrückrufe ab oder legt sie fest.|
| [auto_fitter_options](/cells/de/python-net/aspose.cells/txtloadoptions/auto_fitter_options) | Ruft die Autofitter-Optionen ab und legt sie fest|
| [auto_filter](/cells/de/python-net/aspose.cells/txtloadoptions/auto_filter) | Gibt an, ob die Daten beim Laden der Dateien automatisch gefiltert werden.|
| [font_configs](/cells/de/python-net/aspose.cells/txtloadoptions/font_configs) | Ruft individuelle Schriftartkonfigurationen ab und legt sie fest.<br/> Funktioniert nur für die [Workbook](/cells/de/python-net/aspose.cells/workbook), die diese [LoadOptions](/cells/de/python-net/aspose.cells/loadoptions) zum Laden verwendet.|
| [encoding](/cells/de/python-net/aspose.cells/txtloadoptions/encoding) | Ruft die Standardcodierung ab und legt sie fest.|
| [load_style_strategy](/cells/de/python-net/aspose.cells/txtloadoptions/load_style_strategy) |Gibt die Strategie zum Anwenden des Stils für geparste Werte beim Konvertieren von Zeichenfolgenwerten in Zahlen oder Datumsangaben an.|
| [convert_numeric_data](/cells/de/python-net/aspose.cells/txtloadoptions/convert_numeric_data) | Ruft einen Wert ab, der angibt, ob die Zeichenfolge in der Textdatei in numerische Daten konvertiert wird, oder legt diesen fest.|
| [convert_date_time_data](/cells/de/python-net/aspose.cells/txtloadoptions/convert_date_time_data) | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob die Zeichenfolge in der Textdatei in Datumsdaten konvertiert wird.|
| [keep_precision](/cells/de/python-net/aspose.cells/txtloadoptions/keep_precision) | Gibt an, ob ein Zeichenfolgenwert bei einer Länge von 15 nicht analysiert wird.|
| [separator](/cells/de/python-net/aspose.cells/txtloadoptions/separator) | Ruft das Zeichentrennzeichen der Textdatei ab und legt es fest.|
| [separator_string](/cells/de/python-net/aspose.cells/txtloadoptions/separator_string) | Ruft einen Zeichenfolgenwert als Trennzeichen ab und legt ihn fest.|
| [is_multi_encoded](/cells/de/python-net/aspose.cells/txtloadoptions/is_multi_encoded) | True bedeutet, dass die Datei mehrere Kodierungen enthält.|
| [preferred_parsers](/cells/de/python-net/aspose.cells/txtloadoptions/preferred_parsers) |Ruft bevorzugte Wertparser zum Laden von Textdateien ab und legt diese fest.|
| [has_formula](/cells/de/python-net/aspose.cells/txtloadoptions/has_formula) | Gibt an, ob der Text eine Formel ist, wenn er mit "=" beginnt.|
| [has_text_qualifier](/cells/de/python-net/aspose.cells/txtloadoptions/has_text_qualifier) | Gibt an, ob ein Textqualifizierer für den Zellenwert vorhanden ist. Der Standardwert ist „true“.|
| [text_qualifier](/cells/de/python-net/aspose.cells/txtloadoptions/text_qualifier) | Gibt den Textbezeichner für Zellenwerte an. Der Standardbezeichner ist „““.|
| [treat_consecutive_delimiters_as_one](/cells/de/python-net/aspose.cells/txtloadoptions/treat_consecutive_delimiters_as_one) | Ob aufeinanderfolgende Trennzeichen als eines behandelt werden sollen.|
| [treat_quote_prefix_as_value](/cells/de/python-net/aspose.cells/txtloadoptions/treat_quote_prefix_as_value) | Gibt an, ob das führende einfache Anführungszeichen als Teil des Werts einer Zelle verwendet werden soll.<br/>Der Standardwert ist wahr. Wenn er falsch ist, wird das führende einfache Anführungszeichen aus dem Wert der entsprechenden Zelle entfernt<br/> und [Style.quote_prefix](/cells/de/python-net/aspose.cells/style#quote_prefix) wird für die Zelle auf wahr gesetzt.|
| [extend_to_next_sheet](/cells/de/python-net/aspose.cells/txtloadoptions/extend_to_next_sheet) | Ob Daten auf das nächste Blatt erweitert werden, wenn die Datenzeilen oder -spalten das Limit überschreiten.<br/>Wenn diese Eigenschaft wahr ist, werden zusätzliche Daten auf das nächste Blatt hinter dem aktuellen erweitert (wenn das aktuelle Blatt das letzte ist,<br/>neues Blatt wird an aktuelle Arbeitsmappe angehängt).<br/>Wenn diese Eigenschaft falsch ist, wird die Datenüberschreitung ignoriert.<br/> Standard ist falsch;|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [set_paper_size(type)](/cells/de/python-net/aspose.cells/txtloadoptions/set_paper_size/#PaperSizeType) | Legt das Standarddruckpapierformat aus der Standarddruckereinstellung fest.|



###  Siehe auch
* Modul [aspose.cells](..)
* Klasse [AbstractTextLoadOptions](/cells/de/python-net/aspose.cells/abstracttextloadoptions)
* Klasse [LoadOptions](/cells/de/python-net/aspose.cells/loadoptions)
* Klasse [TxtLoadOptions](/cells/de/python-net/aspose.cells/txtloadoptions)
* Klasse [Workbook](/cells/de/python-net/aspose.cells/workbook)
