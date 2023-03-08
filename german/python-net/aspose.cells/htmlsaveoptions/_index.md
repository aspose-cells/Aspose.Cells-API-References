---
title: HtmlSaveOptions Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 780
url: /de/python-net/aspose.cells/htmlsaveoptions/
is_root: false
---
##  HtmlSaveOptions Klasse
Repräsentiert die Optionen zum Speichern der HTML-Datei.



**Nachlass:** [HtmlSaveOptions](/cells/python-net/aspose.cells/htmlsaveoptions) → 
[SaveOptions](/cells/de/python-net/aspose.cells/saveoptions)



Der Typ HtmlSaveOptions macht die folgenden Member verfügbar:

###  Konstrukteure
| Konstrukteur| Beschreibung|
| :- | :- |
| [HtmlSaveOptions()](/cells/de/python-net/aspose.cells/htmlsaveoptions/__init__/#) | Erstellt Optionen zum Speichern von HTML-Dateien.|
| [HtmlSaveOptions(format)](/cells/de/python-net/aspose.cells/htmlsaveoptions/__init__/#SaveFormat) | Erstellt Optionen zum Speichern von HTML-Dateien.|


###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [save_format](/cells/de/python-net/aspose.cells/htmlsaveoptions/save_format) | Ruft das Sicherungsdateiformat ab.|
| [clear_data](/cells/de/python-net/aspose.cells/htmlsaveoptions/clear_data) | Machen Sie die Arbeitsmappe nach dem Speichern der Datei leer.|
| [cached_file_folder](/cells/de/python-net/aspose.cells/htmlsaveoptions/cached_file_folder) | Der zwischengespeicherte Dateiordner wird verwendet, um einige große Daten zu speichern.|
| [validate_merged_areas](/cells/de/python-net/aspose.cells/htmlsaveoptions/validate_merged_areas) | Gibt an, ob verbundene Zellen vor dem Speichern der Datei validiert werden sollen.|
| [merge_areas](/cells/de/python-net/aspose.cells/htmlsaveoptions/merge_areas) | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden sollen.|
| [create_directory](/cells/de/python-net/aspose.cells/htmlsaveoptions/create_directory) | Wenn wahr und das Verzeichnis nicht existiert, wird das Verzeichnis automatisch erstellt, bevor die Datei gespeichert wird.|
| [sort_names](/cells/de/python-net/aspose.cells/htmlsaveoptions/sort_names) | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden.|
| [sort_external_names](/cells/de/python-net/aspose.cells/htmlsaveoptions/sort_external_names) | Gibt an, ob extern definierte Namen vor dem Speichern der Datei sortiert werden.|
| [refresh_chart_cache](/cells/de/python-net/aspose.cells/htmlsaveoptions/refresh_chart_cache) |Gibt an, ob Diagramm-Cache-Daten aktualisiert werden|
| [warning_callback](/cells/de/python-net/aspose.cells/htmlsaveoptions/warning_callback) | Ruft einen Warnungsrückruf ab oder legt ihn fest.|
| [update_smart_art](/cells/de/python-net/aspose.cells/htmlsaveoptions/update_smart_art) | Gibt an, ob die SmartArt-Einstellung aktualisiert wird.<br/> Der Standardwert ist falsch.|
| [ignore_invisible_shapes](/cells/de/python-net/aspose.cells/htmlsaveoptions/ignore_invisible_shapes) | Geben Sie an, ob diese nicht sichtbaren Formen exportiert werden|
| [page_title](/cells/de/python-net/aspose.cells/htmlsaveoptions/page_title) | Der Titel der HTML-Seite.<br/> Nur zum Speichern im HTML-Stream.|
| [attached_files_directory](/cells/de/python-net/aspose.cells/htmlsaveoptions/attached_files_directory) |Das Verzeichnis, in dem die angehängten Dateien gespeichert werden.<br/> Nur zum Speichern im HTML-Stream.|
| [attached_files_url_prefix](/cells/de/python-net/aspose.cells/htmlsaveoptions/attached_files_url_prefix) | Geben Sie das URL-Präfix von angehängten Dateien wie Bild in der HTML-Datei an.<br/> Nur zum Speichern im HTML-Stream.|
| [default_font_name](/cells/de/python-net/aspose.cells/htmlsaveoptions/default_font_name) | Geben Sie den Namen der Standardschriftart für den HTML-Export an. Die Standardschriftart wird verwendet, wenn die Schriftart des Stils nicht vorhanden ist.<br/>Wenn diese Eigenschaft null ist, verwendet Aspose.Cells eine universelle Schriftart, die dieselbe Familie wie die ursprüngliche Schriftart hat.<br/> der Standardwert ist null.|
| [worksheet_scalable](/cells/de/python-net/aspose.cells/htmlsaveoptions/worksheet_scalable) |Gibt an, ob das HTML über die Zoomstufe des Arbeitsblatts beim Speichern der Datei in HTML vergrößert oder verkleinert wird, der Standardwert ist falsch.|
| [is_export_comments](/cells/de/python-net/aspose.cells/htmlsaveoptions/is_export_comments) | Gibt an, dass beim Exportieren von Kommentaren beim Speichern der Datei in HTML der Standardwert „false“ ist.|
| [export_comments_type](/cells/de/python-net/aspose.cells/htmlsaveoptions/export_comments_type) | Stellt die Art des Exportierens von Kommentaren in HTML-Dateien dar.|
| [disable_downlevel_revealed_comments](/cells/de/python-net/aspose.cells/htmlsaveoptions/disable_downlevel_revealed_comments) | Gibt an, ob beim Exportieren der Datei in HTML bedingte Kommentare von Downlevel deaktiviert werden sollen, der Standardwert ist „false“.|
| [is_exp_image_to_temp_dir](/cells/de/python-net/aspose.cells/htmlsaveoptions/is_exp_image_to_temp_dir) | Gibt an, ob Bilddateien in das temporäre Verzeichnis exportiert werden.<br/> Nur zum Speichern im HTML-Stream.|
| [image_scalable](/cells/de/python-net/aspose.cells/htmlsaveoptions/image_scalable) | Gibt an, ob eine skalierbare Einheit zur Beschreibung der Bildbreite verwendet wird<br/>bei Verwendung einer skalierbaren Einheit zur Beschreibung der Spaltenbreite.<br/> Der Standardwert ist wahr.|
| [width_scalable](/cells/de/python-net/aspose.cells/htmlsaveoptions/width_scalable) | Gibt an, ob eine skalierbare Einheit verwendet wird, um die Spaltenbreite beim Exportieren der Datei in HTML zu beschreiben.<br/> Der Standardwert ist falsch.|
| [export_single_tab](/cells/de/python-net/aspose.cells/htmlsaveoptions/export_single_tab) | Gibt an, ob die einzelne Registerkarte exportiert wird, wenn die Datei nur ein Arbeitsblatt enthält.<br/> Der Standardwert ist falsch.|
| [export_images_as_base64](/cells/de/python-net/aspose.cells/htmlsaveoptions/export_images_as_base64) | Gibt an, ob Bilder im Base64-Format in HTML, MHTML oder EPUB gespeichert werden.|
| [export_active_worksheet_only](/cells/de/python-net/aspose.cells/htmlsaveoptions/export_active_worksheet_only) | Gibt an, ob die gesamte Arbeitsmappe in eine HTML-Datei exportiert wird.|
| [export_print_area_only](/cells/de/python-net/aspose.cells/htmlsaveoptions/export_print_area_only) | Gibt an, ob nur der Druckbereich in eine HTML-Datei exportiert wird. Der Standardwert ist falsch.|
| [export_area](/cells/de/python-net/aspose.cells/htmlsaveoptions/export_area) | Ruft die exportierende CellArea des aktuell aktiven Arbeitsblatts ab oder legt sie fest.<br/>Wenn Sie dieses Attribut setzen, wird der Druckbereich des aktuell aktiven Arbeitsblatts weggelassen.<br/> Beim Speichern der Datei im HTML-Format wird nur der angegebene Bereich exportiert.|
| [parse_html_tag_in_cell](/cells/de/python-net/aspose.cells/htmlsaveoptions/parse_html_tag_in_cell) | Analysieren Sie das HTML-Tag in der Zelle, z. B. als Zellenwert oder als HTML-Tag, der Standardwert ist wahr|
| [html_cross_string_type](/cells/de/python-net/aspose.cells/htmlsaveoptions/html_cross_string_type) | Gibt an, ob eine zellenübergreifende Zeichenfolge beim Speichern einer Excel-Datei im HTML-Format auf die gleiche Weise wie MS Excel angezeigt wird.<br/>Standardmäßig ist der Wert Default, daher gibt es für zellenübergreifende Zeichenfolgen kaum einen Unterschied zwischen den HTML-Dateien, die von Aspose.Cells und MS Excel erstellt wurden.<br/>Aber die Leistung beim Erstellen großer HTML-Dateien, wenn der Wert auf Cross gesetzt wird, wäre um ein Vielfaches schneller als die Einstellung auf Default oder Fit2Cell.|
| [hidden_col_display_type](/cells/de/python-net/aspose.cells/htmlsaveoptions/hidden_col_display_type) | Versteckte Spalte (die Breite dieser Spalte ist 0) in Excel, bevor Sie diese im HTML-Format speichern,<br/>wenn HtmlHiddenColDisplayType "Remove" ist, würde die versteckte Spalte nicht ausgegeben,<br/> wenn der Wert "Hidden" ist, würde die Spalte ausgegeben werden, war aber versteckt, der Standardwert ist "Hidden".|
| [hidden_row_display_type](/cells/de/python-net/aspose.cells/htmlsaveoptions/hidden_row_display_type) | Versteckte Zeile (die Höhe dieser Zeile ist 0) in Excel, bevor Sie diese im HTML-Format speichern,<br/>wenn HtmlHiddenRowDisplayType "Remove" ist, würde die versteckte Zeile nicht ausgegeben,<br/> wenn der Wert "Hidden" ist, würde die Zeile ausgegeben werden, aber war versteckt, der Standardwert ist "Hidden".|
| [encoding](/cells/de/python-net/aspose.cells/htmlsaveoptions/encoding) | Wenn nicht festgelegt, verwenden Sie Encoding.UTF8 als Standardcodierungstyp.|
| [export_object_listener](/cells/de/python-net/aspose.cells/htmlsaveoptions/export_object_listener) | Ruft den ExportObjectListener zum Exportieren von Objekten ab oder legt diesen fest.|
| [file_path_provider](/cells/de/python-net/aspose.cells/htmlsaveoptions/file_path_provider) | Ruft den IFilePathProvider zum separaten Exportieren von Arbeitsblättern in HTML ab oder legt diesen fest.|
| [stream_provider](/cells/de/python-net/aspose.cells/htmlsaveoptions/stream_provider) | Ruft den IStreamProvider zum Exportieren von Objekten ab oder legt diesen fest.|
| [image_options](/cells/de/python-net/aspose.cells/htmlsaveoptions/image_options) | Rufen Sie vor dem Exportieren das ImageOrPrintOptions-Objekt ab|
| [save_as_single_file](/cells/de/python-net/aspose.cells/htmlsaveoptions/save_as_single_file) | Gibt an, ob die HTML-Datei als einzelne Datei gespeichert werden soll.<br/> Der Standardwert ist falsch.|
| [show_all_sheets](/cells/de/python-net/aspose.cells/htmlsaveoptions/show_all_sheets) | Gibt an, ob beim Speichern als einzelne HTML-Datei alle Blätter angezeigt werden.|
| [export_page_headers](/cells/de/python-net/aspose.cells/htmlsaveoptions/export_page_headers) | Gibt an, ob Seitenkopfzeilen exportiert werden.|
| [export_page_footers](/cells/de/python-net/aspose.cells/htmlsaveoptions/export_page_footers) | Gibt an, ob Seitenkopfzeilen exportiert werden.|
| [export_hidden_worksheet](/cells/de/python-net/aspose.cells/htmlsaveoptions/export_hidden_worksheet) |Gibt an, ob der Inhalt des ausgeblendeten Arbeitsblatts exportiert wird. Der Standardwert ist wahr.|
| [presentation_preference](/cells/de/python-net/aspose.cells/htmlsaveoptions/presentation_preference) | Gibt an, ob HTML- oder MHT-Datei die Präsentationspräferenz ist.<br/>Der Standardwert ist falsch.<br/> Wenn Sie eine schönere Präsentation wünschen, setzen Sie den Wert bitte auf true.|
| [cell_css_prefix](/cells/de/python-net/aspose.cells/htmlsaveoptions/cell_css_prefix) | Ruft das Präfix des CSS-Namens ab und legt es fest, der Standardwert ist "".|
| [table_css_id](/cells/de/python-net/aspose.cells/htmlsaveoptions/table_css_id) |Ruft das Präfix des Typs CSS-Namen ab und legt es fest, z. B. tr, col, td usw. Sie sind im Tabellenelement enthalten<br/> die das spezifische TableCssId-Attribut hat. Der Standardwert ist "".|
| [is_full_path_link](/cells/de/python-net/aspose.cells/htmlsaveoptions/is_full_path_link) | Gibt an, ob ein vollständiger Pfadlink in sheet00x.htm, filelist.xml und tabstrip.htm verwendet wird.<br/> Der Standardwert ist falsch.|
| [export_worksheet_css_separately](/cells/de/python-net/aspose.cells/htmlsaveoptions/export_worksheet_css_separately) | Gibt an, ob das Arbeitsblatt-CSS separat exportiert werden soll. Der Standardwert ist „false“.|
| [export_similar_border_style](/cells/de/python-net/aspose.cells/htmlsaveoptions/export_similar_border_style) | Gibt an, ob der ähnliche Rahmenstil exportiert wird, wenn der Rahmenstil von Browsern nicht unterstützt wird.<br/>Wenn Sie die HTML- oder MHT-Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei.<br/> Der Standardwert ist falsch.|
| [merge_empty_td_forcely](/cells/de/python-net/aspose.cells/htmlsaveoptions/merge_empty_td_forcely) | Gibt an, ob leere TD-Elemente beim Exportieren der Datei in HTML zwangsweise zusammengeführt werden.<br/> Die Größe der HTML-Datei wird erheblich reduziert, nachdem der Wert auf true gesetzt wurde. Der Standardwert ist falsch.<br/> Wenn Sie die HTML-Datei in Excel importieren oder perfekte Gitterlinien exportieren möchten, wenn Sie die Datei in HTML speichern,<br/> Bitte behalten Sie den Standardwert bei.|
| [export_cell_coordinate](/cells/de/python-net/aspose.cells/htmlsaveoptions/export_cell_coordinate) | Gibt an, ob beim Speichern der Datei in HTML Excel-Koordinaten von nicht leeren Zellen exportiert werden. Der Standardwert ist falsch.<br/> Wenn Sie die HTML-Ausgabe in Excel importieren möchten, behalten Sie bitte den Standardwert bei.|
| [export_extra_headings](/cells/de/python-net/aspose.cells/htmlsaveoptions/export_extra_headings) | Gibt an, ob zusätzliche Überschriften exportiert werden, wenn die Textlänge länger als die maximale Anzeigespalte ist.<br/> Der Standardwert ist falsch. Wenn Sie die HTML-Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei.|
| [export_headings](/cells/de/python-net/aspose.cells/htmlsaveoptions/export_headings) | Gibt an, ob beim Speichern in HTML-Dateien die Zeilen- und Spaltenüberschriften des Blatts exportiert werden.|
| [export_row_column_headings](/cells/de/python-net/aspose.cells/htmlsaveoptions/export_row_column_headings) | Gibt an, ob beim Speichern in HTML-Dateien die Zeilen- und Spaltenüberschriften des Blatts exportiert werden.|
| [export_formula](/cells/de/python-net/aspose.cells/htmlsaveoptions/export_formula) | Gibt an, ob die Formel beim Speichern der Datei in HTML exportiert wird. Der Standardwert ist wahr.<br/> Wenn Sie die HTML-Ausgabe in Excel importieren möchten, behalten Sie bitte den Standardwert bei.|
| [add_tooltip_text](/cells/de/python-net/aspose.cells/htmlsaveoptions/add_tooltip_text) |Gibt an, ob QuickInfo-Text hinzugefügt wird, wenn die Daten nicht vollständig angezeigt werden können.<br/> Der Standardwert ist falsch.|
| [export_grid_lines](/cells/de/python-net/aspose.cells/htmlsaveoptions/export_grid_lines) | Gibt an, ob die Gitternetzlinien exportiert werden. Der Standardwert ist „false“.|
| [export_bogus_row_data](/cells/de/python-net/aspose.cells/htmlsaveoptions/export_bogus_row_data) | Gibt an, ob falsche Daten in der unteren Zeile exportiert werden. Der Standardwert ist true. Wenn Sie die HTML- oder MHT-Datei importieren möchten<br/> um zu übertreffen, behalten Sie bitte den Standardwert bei.|
| [exclude_unused_styles](/cells/de/python-net/aspose.cells/htmlsaveoptions/exclude_unused_styles) | Gibt an, ob nicht verwendete Stile ausgeschlossen werden.<br/>Bei den generierten HTML-Dateien kann das Ausschließen nicht verwendeter Stile die Dateigröße verringern<br/>ohne die visuellen Effekte zu beeinträchtigen. Der Standardwert dieser Eigenschaft ist also true.<br/>Wenn der Benutzer alle Stile in der Arbeitsmappe für den generierten HTML-Code behalten muss (z. B. das Szenario, in dem der Benutzer<br/> muss die Arbeitsmappe später aus dem generierten HTML-Code wiederherstellen), setzen Sie diese Eigenschaft bitte auf „false“.|
| [export_document_properties](/cells/de/python-net/aspose.cells/htmlsaveoptions/export_document_properties) | Gibt an, ob Dokumenteigenschaften exportiert werden. Der Standardwert ist wahr. Wenn Sie importieren möchten<br/> B. die HTML- oder MHT-Datei nach Excel, behalten Sie bitte den Standardwert bei.|
| [export_worksheet_properties](/cells/de/python-net/aspose.cells/htmlsaveoptions/export_worksheet_properties) | Gibt an, ob Arbeitsblatteigenschaften exportiert werden. Der Standardwert ist wahr. Wenn Sie importieren möchten<br/> B. die HTML- oder MHT-Datei nach Excel, behalten Sie bitte den Standardwert bei.|
| [export_workbook_properties](/cells/de/python-net/aspose.cells/htmlsaveoptions/export_workbook_properties) | Gibt an, ob Arbeitsmappeneigenschaften exportiert werden. Der Standardwert ist wahr. Wenn Sie importieren möchten<br/> B. die HTML- oder MHT-Datei nach Excel, behalten Sie bitte den Standardwert bei.|
| [export_frame_scripts_and_properties](/cells/de/python-net/aspose.cells/htmlsaveoptions/export_frame_scripts_and_properties) | Gibt an, ob Rahmenskripte und Dokumenteigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML- oder MHT-Datei importieren möchten<br/> um zu übertreffen, behalten Sie bitte den Standardwert bei.|
| [export_data_options](/cells/de/python-net/aspose.cells/htmlsaveoptions/export_data_options) | Gibt die Regel zum Exportieren von HTML-Dateidaten an. Der Standardwert ist Alle.|
| [link_target_type](/cells/de/python-net/aspose.cells/htmlsaveoptions/link_target_type) | Angabe des Typs des Zielattributs in<a> link,Der Standardwert ist HtmlLinkTargetType.Parent.|



###  Siehe auch
* Modul [aspose.cells](..)
* Klasse [HtmlSaveOptions](/cells/de/python-net/aspose.cells/htmlsaveoptions)
* Klasse [SaveOptions](/cells/de/python-net/aspose.cells/saveoptions)
