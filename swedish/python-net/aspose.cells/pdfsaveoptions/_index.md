---
title: PdfSaveOptions klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 1180
url: /sv/python-net/aspose.cells/pdfsaveoptions/
is_root: false
---
##  PdfSaveOptions klass
Representerar alternativen för att spara pdf-fil.



**Arv:** [PdfSaveOptions](/cells/python-net/aspose.cells/pdfsaveoptions) → 
[PaginatedSaveOptions](/cells/python-net/aspose.cells/paginatedsaveoptions) → 
[SaveOptions](/cells/sv/python-net/aspose.cells/saveoptions)



Typen PdfSaveOptions avslöjar följande medlemmar:

###  Konstruktörer
| Konstruktör| Beskrivning|
| :- | :- |
| [PdfSaveOptions()](/cells/sv/python-net/aspose.cells/pdfsaveoptions/__init__/#) | Skapar alternativen för att spara pdf-fil.|


###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [save_format](/cells/sv/python-net/aspose.cells/pdfsaveoptions/save_format) | Hämtar spara filformatet.|
| [clear_data](/cells/sv/python-net/aspose.cells/pdfsaveoptions/clear_data) | Gör arbetsboken tom efter att du har sparat filen.|
| [cached_file_folder](/cells/sv/python-net/aspose.cells/pdfsaveoptions/cached_file_folder) | Den cachade filmappen används för att lagra en del stora data.|
| [validate_merged_areas](/cells/sv/python-net/aspose.cells/pdfsaveoptions/validate_merged_areas) | Anger om sammanslagna celler ska valideras innan filen sparas.|
| [merge_areas](/cells/sv/python-net/aspose.cells/pdfsaveoptions/merge_areas) | Anger om områdena för villkorlig formatering och validering ska slås samman innan filen sparas.|
| [create_directory](/cells/sv/python-net/aspose.cells/pdfsaveoptions/create_directory) | Om sant och katalogen inte finns skapas katalogen automatiskt innan filen sparas.|
| [sort_names](/cells/sv/python-net/aspose.cells/pdfsaveoptions/sort_names) | Anger om du sorterar definierade namn innan filen sparas.|
| [sort_external_names](/cells/sv/python-net/aspose.cells/pdfsaveoptions/sort_external_names) | Anger om externt definierade namn sorteras innan filen sparas.|
| [refresh_chart_cache](/cells/sv/python-net/aspose.cells/pdfsaveoptions/refresh_chart_cache) |Anger om diagramcachedata uppdateras|
| [warning_callback](/cells/sv/python-net/aspose.cells/pdfsaveoptions/warning_callback) | Får eller ställer in varningsåteruppringning.|
| [update_smart_art](/cells/sv/python-net/aspose.cells/pdfsaveoptions/update_smart_art) | Indikerar om inställningen för smart konst uppdateras.<br/> Standardvärdet är falskt.|
| [default_font](/cells/sv/python-net/aspose.cells/pdfsaveoptions/default_font) | När tecken i Excel är Unicode och inte är inställda med korrekt typsnitt i cellstil,<br/>De kan visas som block i pdf, bild.<br/>Ställ in standardteckensnittet som MingLiu eller MS Gothic för att visa dessa tecken.<br/> Om den här egenskapen inte är inställd kommer Aspose.Cells att använda systemets standardteckensnitt för att visa dessa unicode-tecken.|
| [check_workbook_default_font](/cells/sv/python-net/aspose.cells/pdfsaveoptions/check_workbook_default_font) | När tecken i Excel är Unicode och inte är inställda med korrekt typsnitt i cellstil,<br/>De kan visas som block i pdf, bild.<br/> Ställ in detta på sant för att försöka använda arbetsbokens standardteckensnitt för att visa dessa tecken först.|
| [check_font_compatibility](/cells/sv/python-net/aspose.cells/pdfsaveoptions/check_font_compatibility) | Anger om teckensnittskompatibilitet ska kontrolleras för varje tecken i texten.|
| [is_font_substitution_char_granularity](/cells/sv/python-net/aspose.cells/pdfsaveoptions/is_font_substitution_char_granularity) | Indikerar om teckensnittet endast ska bytas ut när cellteckensnittet inte är kompatibelt med det.|
| [one_page_per_sheet](/cells/sv/python-net/aspose.cells/pdfsaveoptions/one_page_per_sheet) | Om OnePagePerSheet är sant , kommer allt innehåll på ett ark endast att matas ut till en sida som resultat.<br/> Pappersstorleken för sidinställningarna kommer att vara ogiltig, och de andra inställningarna för sidinställningarna<br/> kommer fortfarande att träda i kraft.|
| [all_columns_in_one_page_per_sheet](/cells/sv/python-net/aspose.cells/pdfsaveoptions/all_columns_in_one_page_per_sheet) | Om AllColumnsInOnePagePerSheet är sant , kommer allt kolumninnehåll i ett ark att matas ut till endast en sida i resultat.<br/> Bredden på pappersstorleken för sidinställningarna ignoreras, och de andra inställningarna för sidinställningarna<br/> kommer fortfarande att träda i kraft.|
| [ignore_error](/cells/sv/python-net/aspose.cells/pdfsaveoptions/ignore_error) | Indikerar om du behöver dölja felet under renderingen.<br/> Felet kan vara fel i form, bild, diagramrendering, etc.|
| [output_blank_page_when_nothing_to_print](/cells/sv/python-net/aspose.cells/pdfsaveoptions/output_blank_page_when_nothing_to_print) | Indikerar om en tom sida ska matas ut när det inte finns något att skriva ut.|
| [page_index](/cells/sv/python-net/aspose.cells/pdfsaveoptions/page_index) | Hämtar eller ställer in det 0-baserade indexet för den första sidan som ska sparas.|
| [page_count](/cells/sv/python-net/aspose.cells/pdfsaveoptions/page_count) | Hämtar eller ställer in antalet sidor som ska sparas.|
| [printing_page_type](/cells/sv/python-net/aspose.cells/pdfsaveoptions/printing_page_type) | Indikerar vilka sidor som inte kommer att skrivas ut.|
| [gridline_type](/cells/sv/python-net/aspose.cells/pdfsaveoptions/gridline_type) | Hämtar eller ställer in rutnätstyp.|
| [text_cross_type](/cells/sv/python-net/aspose.cells/pdfsaveoptions/text_cross_type) | Hämtar eller ställer in visning av texttyp när textbredden är större än cellbredden.|
| [default_edit_language](/cells/sv/python-net/aspose.cells/pdfsaveoptions/default_edit_language) | Hämtar eller ställer in standardspråk för redigering.|
| [sheet_set](/cells/sv/python-net/aspose.cells/pdfsaveoptions/sheet_set) |Hämtar eller ställer in arken att rendera. Standard är alla synliga ark i arbetsboken: [SheetSet.visible](/cells/sv/python-net/aspose.cells.rendering/sheetset#visible).|
| [draw_object_event_handler](/cells/sv/python-net/aspose.cells/pdfsaveoptions/draw_object_event_handler) | Implementerar detta gränssnitt för att få DrawObject och Bound vid rendering.|
| [page_saving_callback](/cells/sv/python-net/aspose.cells/pdfsaveoptions/page_saving_callback) |Kontrollera/indikera framsteg för sidsparprocessen.|
| [embed_standard_windows_fonts](/cells/sv/python-net/aspose.cells/pdfsaveoptions/embed_standard_windows_fonts) | True att bädda in true type-teckensnitt.<br/>Påverkar endast ASCII-tecken 32-127.<br/>Teckensnitt för teckenkoder större än 127 är alltid inbäddade.<br/>Teckensnitt är alltid inbäddade för PDF/A-1a, PDF/A-1b standard.<br/> Standard är sant.|
| [bookmark](/cells/sv/python-net/aspose.cells/pdfsaveoptions/bookmark) | Hämtar och ställer in objektet [PdfBookmarkEntry](/cells/sv/python-net/aspose.cells.rendering/pdfbookmarkentry).|
| [compliance](/cells/sv/python-net/aspose.cells/pdfsaveoptions/compliance) | Arbetsboken konverteras till pdf enligt PdfCompliance i den här egenskapen.|
| [security_options](/cells/sv/python-net/aspose.cells/pdfsaveoptions/security_options) | Ställ in detta alternativ när säkerhet behövs i xls2pdf-resultat.|
| [image_type](/cells/sv/python-net/aspose.cells/pdfsaveoptions/image_type) | Representerar bildtypen vid konvertering av diagram och form.|
| [calculate_formula](/cells/sv/python-net/aspose.cells/pdfsaveoptions/calculate_formula) | Indikerar om formler ska beräknas innan pdf-filen sparas.|
| [pdf_compression](/cells/sv/python-net/aspose.cells/pdfsaveoptions/pdf_compression) |Ange komprimeringsalgoritmen|
| [created_time](/cells/sv/python-net/aspose.cells/pdfsaveoptions/created_time) | Hämtar och ställer in tiden för generering av pdf-dokumentet.|
| [producer](/cells/sv/python-net/aspose.cells/pdfsaveoptions/producer) | Hämtar och ställer in producent av genererade pdf-dokument.|
| [optimization_type](/cells/sv/python-net/aspose.cells/pdfsaveoptions/optimization_type) | Hämtar och ställer in pdf-optimeringstyp.|
| [custom_properties_export](/cells/sv/python-net/aspose.cells/pdfsaveoptions/custom_properties_export) | Hämtar eller ställer in ett värde som bestämmer hur [CustomDocumentPropertyCollection](/cells/sv/python-net/aspose.cells.properties/customdocumentpropertycollection) exporteras till filen PDF. Standardvärdet är None.|
| [export_document_structure](/cells/sv/python-net/aspose.cells/pdfsaveoptions/export_document_structure) | Indikerar om dokumentstruktur ska exporteras.|
| [emf_render_setting](/cells/sv/python-net/aspose.cells/pdfsaveoptions/emf_render_setting) | Inställning för rendering av Emf-metafil.|
| [display_doc_title](/cells/sv/python-net/aspose.cells/pdfsaveoptions/display_doc_title) | Indikerar om fönstrets namnlist ska visa dokumentets titel.|
| [font_encoding](/cells/sv/python-net/aspose.cells/pdfsaveoptions/font_encoding) | Hämtar eller ställer in inbäddad teckensnittskodning i pdf.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [set_image_resample(desired_ppi, jpeg_quality)](/cells/sv/python-net/aspose.cells/pdfsaveoptions/set_image_resample/#int-int) | Ställer in önskad PPI (pixlar per tum) för omsamplingsbilder och jpeg-kvalitet.<br/> Alla bilder kommer att konverteras till JPEG med den angivna kvalitetsinställningen,<br/>och bilder som är större än den angivna PPI (pixlar per tum) omsamplas.|



###  Se även
* modul [aspose.cells](..)
* klass [CustomDocumentPropertyCollection](/cells/sv/python-net/aspose.cells.properties/customdocumentpropertycollection)
* klass [PaginatedSaveOptions](/cells/sv/python-net/aspose.cells/paginatedsaveoptions)
* klass [PdfBookmarkEntry](/cells/sv/python-net/aspose.cells.rendering/pdfbookmarkentry)
* klass [PdfSaveOptions](/cells/sv/python-net/aspose.cells/pdfsaveoptions)
* klass [SaveOptions](/cells/sv/python-net/aspose.cells/saveoptions)
