---
title: ImageOrPrintOptions Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 40
url: /de/python-net/aspose.cells.rendering/imageorprintoptions/
is_root: false
---
##  ImageOrPrintOptions Klasse
Ermöglicht das Festlegen von Optionen beim Rendern von Arbeitsblättern in Bilder, beim Drucken von Arbeitsblättern oder beim Rendern von Diagrammen in Bilder.



Der Typ ImageOrPrintOptions macht die folgenden Member verfügbar:

###  Konstrukteure
| Konstrukteur| Beschreibung|
| :- | :- |
| [ImageOrPrintOptions()](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/__init__/#) | Erstellt eine neue Instanz von ImageOrPrintOptions|


###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [save_format](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/save_format) | Ruft den Formattyp der Ausgabedatei ab oder legt ihn fest<br/> Unterstützen Sie Tiff/XPS|
| [print_with_status_dialog](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/print_with_status_dialog) | Wenn PrintWithStatusDialog = true , wird ein Dialogfeld angezeigt, das den aktuellen Druckstatus anzeigt.<br/> andernfalls wird kein solcher Dialog angezeigt.|
| [horizontal_resolution](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/horizontal_resolution) | Ruft die horizontale Auflösung für generierte Bilder in Punkten pro Zoll ab oder legt diese fest.<br/> Wendet die Bilderzeugungsmethode mit Ausnahme von Bildern im EMF-Format an.|
| [vertical_resolution](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/vertical_resolution) | Ruft die vertikale Auflösung für generierte Bilder in Punkten pro Zoll ab oder legt diese fest.<br/> Wendet die Bilderzeugungsmethode mit Ausnahme von Bildern im EMF-Format an.|
| [tiff_compression](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/tiff_compression) | Ruft den Komprimierungstyp ab oder legt diesen fest, der nur angewendet wird, wenn Seiten im Format `Tiff` gespeichert werden.|
| [tiff_color_depth](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/tiff_color_depth) | Ruft die Bittiefe ab oder legt sie so fest, dass sie nur angewendet wird, wenn Seiten im Format `Tiff` gespeichert werden.|
| [printing_page](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/printing_page) | Gibt an, welche Seiten nicht gedruckt werden.|
| [quality](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/quality) | Ruft einen Wert ab, der die Qualität der generierten Bilder bestimmt, oder legt diesen fest<br/>nur anzuwenden, wenn Seiten im Format `Jpeg` gespeichert werden.|
| [image_type](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/image_type) | Ruft das Format der generierten Bilder ab oder legt es fest.<br/> Standardwert: PNG.|
| [is_cell_auto_fit](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/is_cell_auto_fit) | Gibt an, ob die Breite und Höhe der Zellen automatisch an den Zellenwert angepasst wird.<br/> Der Standardwert ist falsch.|
| [one_page_per_sheet](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/one_page_per_sheet) | Wenn OnePagePerSheet true ist, wird der gesamte Inhalt eines Blatts als Ergebnis nur auf einer Seite ausgegeben.<br/> Die Papiergröße von pagesetup und die anderen Einstellungen von pagesetup werden ungültig<br/> wird noch wirksam.|
| [all_columns_in_one_page_per_sheet](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/all_columns_in_one_page_per_sheet) | Wenn AllColumnsInOnePagePerSheet true ist, werden alle Spalteninhalte eines Blatts als Ergebnis nur auf einer Seite ausgegeben.<br/> Die Breite des Papierformats von pagesetup und die anderen Einstellungen von pagesetup werden ungültig<br/> wird noch wirksam.|
| [draw_object_event_handler](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/draw_object_event_handler) | Implementiert diese Schnittstelle, um DrawObject und Bound beim Rendern abzurufen.|
| [chart_image_type](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/chart_image_type) | Geben Sie beim Konvertieren den Diagrammbildtyp an.<br/> Standardwert: PNG.|
| [embeded_image_name_in_svg](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/embeded_image_name_in_svg) | Geben Sie den Dateinamen des eingebetteten Bildes in svg an.<br/> Dies sollte ein vollständiger Pfad mit einem Verzeichnis wie „c:\\xpsEmbedded“ sein.|
| [svg_fit_to_view_port](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/svg_fit_to_view_port) | Wenn diese Eigenschaft wahr ist, passt das generierte SVG zum Ansichtsport.|
| [only_area](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/only_area) | Wenn diese Eigenschaft wahr ist, wird ein Bereich ausgegeben, und es wird keine Skalierung wirksam.|
| [text_rendering_hint](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/text_rendering_hint) | Gibt die Qualität der Textwiedergabe an.<br/> Der Standardwert ist TextRenderingHint.SystemDefault|
| [smoothing_mode](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/smoothing_mode) | Legt fest, ob Glättung (Antialiasing) auf Linien und Kurven sowie die Kanten gefüllter Bereiche angewendet wird.<br/> Der Standardwert ist SmoothingMode.None|
| [transparent](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/transparent) | Gibt an, ob der Hintergrund des generierten Bildes transparent sein soll.|
| [pixel_format](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/pixel_format) |Ruft das Pixelformat für die generierten Bilder ab oder legt es fest.|
| [warning_callback](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/warning_callback) | Ruft Warnungsrückrufe ab oder legt sie fest.|
| [page_saving_callback](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/page_saving_callback) | Steuerung/Fortschritt des Seitenspeichervorgangs anzeigen.|
| [is_font_substitution_char_granularity](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/is_font_substitution_char_granularity) | Gibt an, ob die Zeichenschrift nur dann ersetzt werden soll, wenn die Zellenschrift nicht damit kompatibel ist.|
| [page_index](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/page_index) | Ruft den 0-basierten Index der ersten zu speichernden Seite ab oder legt diesen fest.|
| [page_count](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/page_count) | Ruft die Anzahl der zu speichernden Seiten ab oder legt diese fest.|
| [is_optimized](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/is_optimized) | Gibt an, ob die Ausgangselemente optimiert werden sollen.|
| [default_font](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/default_font) | Wenn Zeichen in Excel Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt werden,<br/>Sie können als Block in PDF, Bild erscheinen.<br/>Legen Sie die DefaultFont wie MingLiu oder MS Gothic fest, um diese Zeichen anzuzeigen.<br/> Wenn diese Eigenschaft nicht festgelegt ist, verwendet Aspose.Cells die Systemstandardschriftart, um diese Unicode-Zeichen anzuzeigen.|
| [check_workbook_default_font](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/check_workbook_default_font) | Wenn Zeichen in Excel Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt werden,<br/>Sie können als Block in PDF, Bild erscheinen.<br/> Setzen Sie dies auf „true“, um zu versuchen, die Standardschriftart der Arbeitsmappe zu verwenden, um diese Zeichen zuerst anzuzeigen.|
| [output_blank_page_when_nothing_to_print](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/output_blank_page_when_nothing_to_print) | Gibt an, ob eine leere Seite ausgegeben werden soll, wenn nichts zu drucken ist.|
| [gridline_type](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/gridline_type) | Ruft den Rasterlinientyp ab oder legt diesen fest.|
| [text_cross_type](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/text_cross_type) | Ruft die Anzeige des Texttyps ab oder legt diese fest, wenn die Textbreite größer als die Zellenbreite ist.|
| [emf_type](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/emf_type) | Ruft einen EmfType ab oder legt diesen fest, der das Format der Metadatei angibt.<br/> Der Standardwert ist EmfPlusDual.|
| [default_edit_language](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/default_edit_language) | Ruft die Standardbearbeitungssprache ab oder legt sie fest.|
| [sheet_set](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/sheet_set) |Ruft die zu rendernden Blätter ab oder legt sie fest. Standardmäßig sind alle sichtbaren Blätter in der Arbeitsmappe: [SheetSet.visible](/cells/de/python-net/aspose.cells.rendering/sheetset#visible).|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [set_desired_size(desired_width, desired_height)](/cells/de/python-net/aspose.cells.rendering/imageorprintoptions/set_desired_size/#int-int) | Legt die gewünschte Breite und Höhe des Bildes fest.|



###  Beispiele

```python
from aspose.cells import Workbook
from aspose.cells.drawing import ImageType
from aspose.cells.rendering import ImageOrPrintOptions

# Set Image Or Print Options
options = ImageOrPrintOptions()
# Set output image format
options.image_type = ImageType.PNG
# Set Horizontal resolution
options.horizontal_resolution = 300
# Set Vertical Resolution
options.vertical_resolution = 300
# Instantiate Workbook
book = Workbook("test.xls")
# Save chart as Image using ImageOrPrint Options
book.worksheets[0].charts[0].to_image("chart.png", options)

```

###  Siehe auch
* Modul [aspose.cells.rendering](..)
