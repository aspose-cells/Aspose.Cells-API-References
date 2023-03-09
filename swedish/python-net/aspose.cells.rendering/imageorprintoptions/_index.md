---
title: ImageOrPrintOptions klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 40
url: /sv/python-net/aspose.cells.rendering/imageorprintoptions/
is_root: false
---
##  ImageOrPrintOptions klass
Tillåter att ange alternativ när du renderar kalkylblad till bilder, skriver ut kalkylblad eller renderar diagram till bild.



Typen ImageOrPrintOptions avslöjar följande medlemmar:

###  Konstruktörer
| Konstruktör| Beskrivning|
| :- | :- |
| [ImageOrPrintOptions()](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/__init__/#) | Konstruerar en ny instans av ImageOrPrintOptions|


###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [save_format](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/save_format) | Hämtar eller ställer in utdatafilens formattyp<br/> Support Tiff/XPS|
| [print_with_status_dialog](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/print_with_status_dialog) | Om PrintWithStatusDialog = true , kommer det att finnas en dialogruta som visar aktuell utskriftsstatus.<br/> annars visas ingen sådan dialog.|
| [horizontal_resolution](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/horizontal_resolution) |Hämtar eller ställer in den horisontella upplösningen för genererade bilder, i punkter per tum.<br/> Tillämpar genererande bildmetoden förutom bilder i Emf-format.|
| [vertical_resolution](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/vertical_resolution) | Hämtar eller ställer in den vertikala upplösningen för genererade bilder, i punkter per tum.<br/> Tillämpar genererande bildmetod förutom EMF-formatbild.|
| [tiff_compression](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/tiff_compression) | Hämtar eller ställer in typen av komprimering så att den endast tillämpas när sidor sparas i formatet `Tiff`.|
| [tiff_color_depth](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/tiff_color_depth) | Hämtar eller ställer in bitdjup för att endast tillämpas när sidor sparas i formatet `Tiff`.|
| [printing_page](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/printing_page) | Indikerar vilka sidor som inte kommer att skrivas ut.|
| [quality](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/quality) | Hämtar eller ställer in ett värde som bestämmer kvaliteten på de genererade bilderna<br/> gäller endast när du sparar sidor i formatet `Jpeg`. Standardvärdet är 100|
| [image_type](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/image_type) | Hämtar eller ställer in formatet för de genererade bilderna.<br/> standardvärde: PNG.|
| [is_cell_auto_fit](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/is_cell_auto_fit) | Indikerar om bredden och höjden på cellerna automatiskt anpassas efter cellvärde.<br/> Standardvärdet är falskt.|
| [one_page_per_sheet](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/one_page_per_sheet) | Om OnePagePerSheet är sant , kommer allt innehåll på ett ark endast att matas ut till en sida som resultat.<br/> Pappersstorleken för sidinställningarna kommer att vara ogiltig, och de andra inställningarna för sidinställningarna<br/> kommer fortfarande att träda i kraft.|
| [all_columns_in_one_page_per_sheet](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/all_columns_in_one_page_per_sheet) | Om AllColumnsInOnePagePerSheet är sant , kommer allt kolumninnehåll i ett ark att matas ut till endast en sida i resultat.<br/> Bredden på pappersstorleken för sidinställningarna kommer att vara ogiltig, och de andra inställningarna för sidinställningarna<br/> kommer fortfarande att träda i kraft.|
| [draw_object_event_handler](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/draw_object_event_handler) | Implementerar detta gränssnitt för att få DrawObject och Bound vid rendering.|
| [chart_image_type](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/chart_image_type) | Ange diagrambildstyp vid konvertering.<br/> standardvärde: PNG.|
| [embeded_image_name_in_svg](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/embeded_image_name_in_svg) | Ange filnamnet på den inbäddade bilden i svg.<br/> Detta bör vara fullständig sökväg med katalog som "c:\\xpsEmbedded"|
| [svg_fit_to_view_port](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/svg_fit_to_view_port) | om den här egenskapen är sann kommer den genererade svg att passa för att visa port.|
| [only_area](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/only_area) | Om den här egenskapen är sann kommer ett område att matas ut, och ingen skala kommer att träda i kraft.|
| [text_rendering_hint](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/text_rendering_hint) | Anger kvaliteten på textåtergivningen.<br/> Standardvärdet är TextRenderingHint.SystemDefault|
| [smoothing_mode](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/smoothing_mode) | Anger om utjämning (kantutjämning) tillämpas på linjer och kurvor och kanterna på fyllda områden.<br/> Standardvärdet är SmoothingMode.None|
| [transparent](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/transparent) | Indikerar om bakgrunden för den genererade bilden ska vara transparent.|
| [pixel_format](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/pixel_format) | Hämtar eller ställer in pixelformatet för de genererade bilderna.|
| [warning_callback](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/warning_callback) | Får eller ställer in varningsåteruppringning.|
| [page_saving_callback](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/page_saving_callback) |Kontrollera/indikera framsteg för sidsparprocessen.|
| [is_font_substitution_char_granularity](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/is_font_substitution_char_granularity) | Indikerar om teckensnittet endast ska bytas ut när cellteckensnittet inte är kompatibelt med det.|
| [page_index](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/page_index) | Hämtar eller ställer in det 0-baserade indexet för den första sidan som ska sparas.|
| [page_count](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/page_count) | Hämtar eller ställer in antalet sidor som ska sparas.|
| [is_optimized](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/is_optimized) | Indikerar om utgångselementen ska optimeras.|
| [default_font](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/default_font) | När tecken i Excel är Unicode och inte är inställda med korrekt typsnitt i cellstil,<br/>De kan visas som block i pdf, bild.<br/>Ställ in standardteckensnittet som MingLiu eller MS Gothic för att visa dessa tecken.<br/> Om den här egenskapen inte är inställd kommer Aspose.Cells att använda systemets standardteckensnitt för att visa dessa unicode-tecken.|
| [check_workbook_default_font](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/check_workbook_default_font) | När tecken i Excel är Unicode och inte är inställda med korrekt typsnitt i cellstil,<br/>De kan visas som block i pdf, bild.<br/> Ställ in detta på sant för att försöka använda arbetsbokens standardteckensnitt för att visa dessa tecken först.|
| [output_blank_page_when_nothing_to_print](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/output_blank_page_when_nothing_to_print) | Indikerar om en tom sida ska matas ut när det inte finns något att skriva ut.|
| [gridline_type](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/gridline_type) | Hämtar eller ställer in rutnätstyp.|
| [text_cross_type](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/text_cross_type) | Hämtar eller ställer in visning av texttyp när textbredden är större än cellbredden.|
| [emf_type](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/emf_type) | Hämtar eller ställer in en EmfType som anger formatet för metafilen.<br/>Standardvärdet är EmfPlusDual.|
| [default_edit_language](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/default_edit_language) | Hämtar eller ställer in standardspråk för redigering.|
| [sheet_set](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/sheet_set) |Hämtar eller ställer in arken att rendera. Standard är alla synliga ark i arbetsboken: [SheetSet.visible](/cells/sv/python-net/aspose.cells.rendering/sheetset#visible).|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [set_desired_size(desired_width, desired_height)](/cells/sv/python-net/aspose.cells.rendering/imageorprintoptions/set_desired_size/#int-int) | Ställer in önskad bredd och höjd på bilden.|



###  Exempel

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

###  Se även
* modul [aspose.cells.rendering](..)
