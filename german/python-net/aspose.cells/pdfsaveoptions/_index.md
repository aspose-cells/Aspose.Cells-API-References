---
title: PdfSaveOptions Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 1180
url: /de/python-net/aspose.cells/pdfsaveoptions/
is_root: false
---
##  PdfSaveOptions Klasse
Stellt die Optionen zum Speichern von PDF-Dateien dar.



**Nachlass:** [PdfSaveOptions](/cells/python-net/aspose.cells/pdfsaveoptions) → 
[PaginatedSaveOptions](/cells/python-net/aspose.cells/paginatedsaveoptions) → 
[SaveOptions](/cells/de/python-net/aspose.cells/saveoptions)



Der Typ PdfSaveOptions macht die folgenden Member verfügbar:

###  Konstrukteure
| Konstrukteur| Beschreibung|
| :- | :- |
| [PdfSaveOptions()](/cells/de/python-net/aspose.cells/pdfsaveoptions/__init__/#) | Erstellt die Optionen zum Speichern von PDF-Dateien.|


###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [save_format](/cells/de/python-net/aspose.cells/pdfsaveoptions/save_format) | Ruft das Sicherungsdateiformat ab.|
| [clear_data](/cells/de/python-net/aspose.cells/pdfsaveoptions/clear_data) | Machen Sie die Arbeitsmappe nach dem Speichern der Datei leer.|
| [cached_file_folder](/cells/de/python-net/aspose.cells/pdfsaveoptions/cached_file_folder) | Der zwischengespeicherte Dateiordner wird verwendet, um einige große Daten zu speichern.|
| [validate_merged_areas](/cells/de/python-net/aspose.cells/pdfsaveoptions/validate_merged_areas) | Gibt an, ob verbundene Zellen vor dem Speichern der Datei validiert werden sollen.|
| [merge_areas](/cells/de/python-net/aspose.cells/pdfsaveoptions/merge_areas) | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden sollen.|
| [create_directory](/cells/de/python-net/aspose.cells/pdfsaveoptions/create_directory) | Wenn wahr und das Verzeichnis nicht existiert, wird das Verzeichnis automatisch erstellt, bevor die Datei gespeichert wird.|
| [sort_names](/cells/de/python-net/aspose.cells/pdfsaveoptions/sort_names) | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden.|
| [sort_external_names](/cells/de/python-net/aspose.cells/pdfsaveoptions/sort_external_names) | Gibt an, ob extern definierte Namen vor dem Speichern der Datei sortiert werden.|
| [refresh_chart_cache](/cells/de/python-net/aspose.cells/pdfsaveoptions/refresh_chart_cache) |Gibt an, ob Diagramm-Cache-Daten aktualisiert werden|
| [warning_callback](/cells/de/python-net/aspose.cells/pdfsaveoptions/warning_callback) | Ruft einen Warnungsrückruf ab oder legt ihn fest.|
| [update_smart_art](/cells/de/python-net/aspose.cells/pdfsaveoptions/update_smart_art) | Gibt an, ob die SmartArt-Einstellung aktualisiert wird.<br/> Der Standardwert ist falsch.|
| [default_font](/cells/de/python-net/aspose.cells/pdfsaveoptions/default_font) | Wenn Zeichen in Excel Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt werden,<br/>Sie können als Block in PDF, Bild erscheinen.<br/>Legen Sie die DefaultFont wie MingLiu oder MS Gothic fest, um diese Zeichen anzuzeigen.<br/> Wenn diese Eigenschaft nicht festgelegt ist, verwendet Aspose.Cells die Systemstandardschriftart, um diese Unicode-Zeichen anzuzeigen.|
| [check_workbook_default_font](/cells/de/python-net/aspose.cells/pdfsaveoptions/check_workbook_default_font) | Wenn Zeichen in Excel Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt werden,<br/>Sie können als Block in PDF, Bild erscheinen.<br/> Setzen Sie dies auf „true“, um zu versuchen, die Standardschriftart der Arbeitsmappe zu verwenden, um diese Zeichen zuerst anzuzeigen.|
| [check_font_compatibility](/cells/de/python-net/aspose.cells/pdfsaveoptions/check_font_compatibility) | Gibt an, ob die Schriftkompatibilität für jedes Zeichen im Text überprüft werden soll.|
| [is_font_substitution_char_granularity](/cells/de/python-net/aspose.cells/pdfsaveoptions/is_font_substitution_char_granularity) | Gibt an, ob die Zeichenschrift nur dann ersetzt werden soll, wenn die Zellenschrift nicht damit kompatibel ist.|
| [one_page_per_sheet](/cells/de/python-net/aspose.cells/pdfsaveoptions/one_page_per_sheet) | Wenn OnePagePerSheet true ist, wird der gesamte Inhalt eines Blatts als Ergebnis nur auf einer Seite ausgegeben.<br/> Die Papiergröße von pagesetup und die anderen Einstellungen von pagesetup werden ungültig<br/> wird noch wirksam.|
| [all_columns_in_one_page_per_sheet](/cells/de/python-net/aspose.cells/pdfsaveoptions/all_columns_in_one_page_per_sheet) | Wenn AllColumnsInOnePagePerSheet true ist, werden alle Spalteninhalte eines Blatts als Ergebnis nur auf einer Seite ausgegeben.<br/> Die Breite des Papierformats von pagesetup und die anderen Einstellungen von pagesetup werden ignoriert<br/> wird noch wirksam.|
| [ignore_error](/cells/de/python-net/aspose.cells/pdfsaveoptions/ignore_error) | Gibt an, ob Sie den Fehler beim Rendern ausblenden müssen.<br/> Der Fehler kann ein Fehler in Form, Bild, Diagrammwiedergabe usw. sein.|
| [output_blank_page_when_nothing_to_print](/cells/de/python-net/aspose.cells/pdfsaveoptions/output_blank_page_when_nothing_to_print) | Gibt an, ob eine leere Seite ausgegeben werden soll, wenn nichts zu drucken ist.|
| [page_index](/cells/de/python-net/aspose.cells/pdfsaveoptions/page_index) | Ruft den 0-basierten Index der ersten zu speichernden Seite ab oder legt diesen fest.|
| [page_count](/cells/de/python-net/aspose.cells/pdfsaveoptions/page_count) | Ruft die Anzahl der zu speichernden Seiten ab oder legt diese fest.|
| [printing_page_type](/cells/de/python-net/aspose.cells/pdfsaveoptions/printing_page_type) | Gibt an, welche Seiten nicht gedruckt werden.|
| [gridline_type](/cells/de/python-net/aspose.cells/pdfsaveoptions/gridline_type) | Ruft den Rasterlinientyp ab oder legt diesen fest.|
| [text_cross_type](/cells/de/python-net/aspose.cells/pdfsaveoptions/text_cross_type) | Ruft die Anzeige des Texttyps ab oder legt diese fest, wenn die Textbreite größer als die Zellenbreite ist.|
| [default_edit_language](/cells/de/python-net/aspose.cells/pdfsaveoptions/default_edit_language) | Ruft die Standardbearbeitungssprache ab oder legt sie fest.|
| [sheet_set](/cells/de/python-net/aspose.cells/pdfsaveoptions/sheet_set) |Ruft die zu rendernden Blätter ab oder legt diese fest. Standard sind alle sichtbaren Blätter in der Arbeitsmappe: [SheetSet.visible](/cells/de/python-net/aspose.cells.rendering/sheetset#visible).|
| [draw_object_event_handler](/cells/de/python-net/aspose.cells/pdfsaveoptions/draw_object_event_handler) | Implementiert diese Schnittstelle, um DrawObject und Bound beim Rendern abzurufen.|
| [page_saving_callback](/cells/de/python-net/aspose.cells/pdfsaveoptions/page_saving_callback) |Steuerung/Fortschritt des Seitenspeichervorgangs anzeigen.|
| [embed_standard_windows_fonts](/cells/de/python-net/aspose.cells/pdfsaveoptions/embed_standard_windows_fonts) | True zum Einbetten von TrueType-Schriftarten.<br/>Betrifft nur die ASCII-Zeichen 32-127.<br/>Schriftarten für Zeichencodes größer als 127 werden immer eingebettet.<br/>Bei PDF/A-1a, PDF/A-1b Standard sind Schriften immer eingebettet.<br/> Standard ist wahr.|
| [bookmark](/cells/de/python-net/aspose.cells/pdfsaveoptions/bookmark) | Ruft das Objekt [PdfBookmarkEntry](/cells/de/python-net/aspose.cells.rendering/pdfbookmarkentry) ab und legt es fest.|
| [compliance](/cells/de/python-net/aspose.cells/pdfsaveoptions/compliance) | Die Arbeitsmappe wird gemäß PdfCompliance in dieser Eigenschaft in PDF konvertiert.|
| [security_options](/cells/de/python-net/aspose.cells/pdfsaveoptions/security_options) | Stellen Sie diese Optionen ein, wenn Sicherheit im xls2pdf-Ergebnis erforderlich ist.|
| [image_type](/cells/de/python-net/aspose.cells/pdfsaveoptions/image_type) | Stellt den Bildtyp dar, wenn das Diagramm und die Form konvertiert werden.|
| [calculate_formula](/cells/de/python-net/aspose.cells/pdfsaveoptions/calculate_formula) | Gibt an, ob Formeln vor dem Speichern der PDF-Datei berechnet werden sollen.|
| [pdf_compression](/cells/de/python-net/aspose.cells/pdfsaveoptions/pdf_compression) |Geben Sie den Komprimierungsalgorithmus an|
| [created_time](/cells/de/python-net/aspose.cells/pdfsaveoptions/created_time) | Ruft den Zeitpunkt der Generierung des PDF-Dokuments ab und legt ihn fest.|
| [producer](/cells/de/python-net/aspose.cells/pdfsaveoptions/producer) | Ruft den Erzeuger des generierten PDF-Dokuments ab und legt ihn fest.|
| [optimization_type](/cells/de/python-net/aspose.cells/pdfsaveoptions/optimization_type) | Ruft den PDF-Optimierungstyp ab und legt ihn fest.|
| [custom_properties_export](/cells/de/python-net/aspose.cells/pdfsaveoptions/custom_properties_export) | Ruft einen Wert ab oder legt diesen fest, der bestimmt, wie [CustomDocumentPropertyCollection](/cells/de/python-net/aspose.cells.properties/customdocumentpropertycollection) in die PDF-Datei exportiert werden. Der Standardwert ist „Keine“.|
| [export_document_structure](/cells/de/python-net/aspose.cells/pdfsaveoptions/export_document_structure) | Gibt an, ob die Dokumentstruktur exportiert werden soll.|
| [emf_render_setting](/cells/de/python-net/aspose.cells/pdfsaveoptions/emf_render_setting) | Einstellung zum Rendern der EMF-Metadatei.|
| [display_doc_title](/cells/de/python-net/aspose.cells/pdfsaveoptions/display_doc_title) | Gibt an, ob die Titelleiste des Fensters den Dokumenttitel anzeigen soll.|
| [font_encoding](/cells/de/python-net/aspose.cells/pdfsaveoptions/font_encoding) | Ruft die eingebettete Schriftcodierung in PDF ab oder legt sie fest.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [set_image_resample(desired_ppi, jpeg_quality)](/cells/de/python-net/aspose.cells/pdfsaveoptions/set_image_resample/#int-int) | Legt die gewünschte PPI (Pixel pro Zoll) von Resample-Bildern und die JPEG-Qualität fest.<br/> Alle Bilder werden mit der angegebenen Qualitätseinstellung in JPEG konvertiert,<br/>und Bilder, die größer als der angegebene PPI (Pixel pro Zoll) sind, werden neu berechnet.|



###  Siehe auch
* Modul [aspose.cells](..)
* Klasse [CustomDocumentPropertyCollection](/cells/de/python-net/aspose.cells.properties/customdocumentpropertycollection)
* Klasse [PaginatedSaveOptions](/cells/de/python-net/aspose.cells/paginatedsaveoptions)
* Klasse [PdfBookmarkEntry](/cells/de/python-net/aspose.cells.rendering/pdfbookmarkentry)
* Klasse [PdfSaveOptions](/cells/de/python-net/aspose.cells/pdfsaveoptions)
* Klasse [SaveOptions](/cells/de/python-net/aspose.cells/saveoptions)
