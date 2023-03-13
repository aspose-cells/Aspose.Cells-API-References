---
title: PaginatedSaveOptions Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 1150
url: /de/python-net/aspose.cells/paginatedsaveoptions/
is_root: false
---
##  PaginatedSaveOptions Klasse
Stellt die Optionen für die Paginierung dar.



**Nachlass:** [PaginatedSaveOptions](/cells/python-net/aspose.cells/paginatedsaveoptions) → 
[SaveOptions](/cells/de/python-net/aspose.cells/saveoptions)



Der Typ PaginatedSaveOptions macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [save_format](/cells/de/python-net/aspose.cells/paginatedsaveoptions/save_format) | Ruft das Sicherungsdateiformat ab.|
| [clear_data](/cells/de/python-net/aspose.cells/paginatedsaveoptions/clear_data) | Machen Sie die Arbeitsmappe nach dem Speichern der Datei leer.|
| [cached_file_folder](/cells/de/python-net/aspose.cells/paginatedsaveoptions/cached_file_folder) | Der zwischengespeicherte Dateiordner wird verwendet, um einige große Daten zu speichern.|
| [validate_merged_areas](/cells/de/python-net/aspose.cells/paginatedsaveoptions/validate_merged_areas) | Gibt an, ob verbundene Zellen vor dem Speichern der Datei validiert werden sollen.|
| [merge_areas](/cells/de/python-net/aspose.cells/paginatedsaveoptions/merge_areas) | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden sollen.|
| [create_directory](/cells/de/python-net/aspose.cells/paginatedsaveoptions/create_directory) | Wenn wahr und das Verzeichnis nicht existiert, wird das Verzeichnis automatisch erstellt, bevor die Datei gespeichert wird.|
| [sort_names](/cells/de/python-net/aspose.cells/paginatedsaveoptions/sort_names) | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden.|
| [sort_external_names](/cells/de/python-net/aspose.cells/paginatedsaveoptions/sort_external_names) |Gibt an, ob extern definierte Namen vor dem Speichern der Datei sortiert werden.|
| [refresh_chart_cache](/cells/de/python-net/aspose.cells/paginatedsaveoptions/refresh_chart_cache) | Gibt an, ob Diagramm-Cache-Daten aktualisiert werden|
| [warning_callback](/cells/de/python-net/aspose.cells/paginatedsaveoptions/warning_callback) | Ruft einen Warnungsrückruf ab oder legt ihn fest.|
| [update_smart_art](/cells/de/python-net/aspose.cells/paginatedsaveoptions/update_smart_art) | Gibt an, ob die SmartArt-Einstellung aktualisiert wird.<br/> Der Standardwert ist falsch.|
| [default_font](/cells/de/python-net/aspose.cells/paginatedsaveoptions/default_font) | Wenn Zeichen in Excel Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt werden,<br/>Sie können als Block in PDF, Bild erscheinen.<br/>Legen Sie die DefaultFont wie MingLiu oder MS Gothic fest, um diese Zeichen anzuzeigen.<br/> Wenn diese Eigenschaft nicht festgelegt ist, verwendet Aspose.Cells die Systemstandardschriftart, um diese Unicode-Zeichen anzuzeigen.|
| [check_workbook_default_font](/cells/de/python-net/aspose.cells/paginatedsaveoptions/check_workbook_default_font) | Wenn Zeichen in Excel Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt werden,<br/>Sie können als Block in PDF, Bild erscheinen.<br/> Setzen Sie dies auf „true“, um zu versuchen, die Standardschriftart der Arbeitsmappe zu verwenden, um diese Zeichen zuerst anzuzeigen.|
| [check_font_compatibility](/cells/de/python-net/aspose.cells/paginatedsaveoptions/check_font_compatibility) |Gibt an, ob die Schriftkompatibilität für jedes Zeichen im Text überprüft werden soll.|
| [is_font_substitution_char_granularity](/cells/de/python-net/aspose.cells/paginatedsaveoptions/is_font_substitution_char_granularity) | Gibt an, ob die Zeichenschrift nur dann ersetzt werden soll, wenn die Zellenschrift nicht damit kompatibel ist.|
| [one_page_per_sheet](/cells/de/python-net/aspose.cells/paginatedsaveoptions/one_page_per_sheet) | Wenn OnePagePerSheet true ist, wird der gesamte Inhalt eines Blatts als Ergebnis nur auf einer Seite ausgegeben.<br/> Die Papiergröße von pagesetup und die anderen Einstellungen von pagesetup werden ungültig<br/> wird noch wirksam.|
| [all_columns_in_one_page_per_sheet](/cells/de/python-net/aspose.cells/paginatedsaveoptions/all_columns_in_one_page_per_sheet) | Wenn AllColumnsInOnePagePerSheet true ist, werden alle Spalteninhalte eines Blatts als Ergebnis nur auf einer Seite ausgegeben.<br/> Die Breite des Papierformats von pagesetup und die anderen Einstellungen von pagesetup werden ignoriert<br/> wird noch wirksam.|
| [ignore_error](/cells/de/python-net/aspose.cells/paginatedsaveoptions/ignore_error) | Gibt an, ob Sie den Fehler beim Rendern ausblenden müssen.<br/> Der Fehler kann ein Fehler in Form, Bild, Diagrammwiedergabe usw. sein.|
| [output_blank_page_when_nothing_to_print](/cells/de/python-net/aspose.cells/paginatedsaveoptions/output_blank_page_when_nothing_to_print) | Gibt an, ob eine leere Seite ausgegeben werden soll, wenn nichts zu drucken ist.|
| [page_index](/cells/de/python-net/aspose.cells/paginatedsaveoptions/page_index) | Ruft den 0-basierten Index der ersten zu speichernden Seite ab oder legt diesen fest.|
| [page_count](/cells/de/python-net/aspose.cells/paginatedsaveoptions/page_count) | Ruft die Anzahl der zu speichernden Seiten ab oder legt diese fest.|
| [printing_page_type](/cells/de/python-net/aspose.cells/paginatedsaveoptions/printing_page_type) | Gibt an, welche Seiten nicht gedruckt werden.|
| [gridline_type](/cells/de/python-net/aspose.cells/paginatedsaveoptions/gridline_type) | Ruft den Rasterlinientyp ab oder legt diesen fest.|
| [text_cross_type](/cells/de/python-net/aspose.cells/paginatedsaveoptions/text_cross_type) | Ruft die Anzeige des Texttyps ab oder legt diese fest, wenn die Textbreite größer als die Zellenbreite ist.|
| [default_edit_language](/cells/de/python-net/aspose.cells/paginatedsaveoptions/default_edit_language) | Ruft die Standardbearbeitungssprache ab oder legt sie fest.|
| [sheet_set](/cells/de/python-net/aspose.cells/paginatedsaveoptions/sheet_set) |Ruft die zu rendernden Blätter ab oder legt diese fest. Standard sind alle sichtbaren Blätter in der Arbeitsmappe: [SheetSet.visible](/cells/de/python-net/aspose.cells.rendering/sheetset#visible).|
| [draw_object_event_handler](/cells/de/python-net/aspose.cells/paginatedsaveoptions/draw_object_event_handler) | Implementiert diese Schnittstelle, um DrawObject und Bound beim Rendern abzurufen.|
| [page_saving_callback](/cells/de/python-net/aspose.cells/paginatedsaveoptions/page_saving_callback) | Steuerung/Fortschritt des Seitenspeichervorgangs anzeigen.|



###  Siehe auch
* Modul [aspose.cells](..)
* Klasse [PaginatedSaveOptions](/cells/de/python-net/aspose.cells/paginatedsaveoptions)
* Klasse [SaveOptions](/cells/de/python-net/aspose.cells/saveoptions)
