---
title: HtmlSaveOptions klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 780
url: /sv/python-net/aspose.cells/htmlsaveoptions/
is_root: false
---
##  HtmlSaveOptions klass
Representerar alternativen för att spara html-fil.



**Arv:** [HtmlSaveOptions](/cells/python-net/aspose.cells/htmlsaveoptions) → 
[SaveOptions](/cells/sv/python-net/aspose.cells/saveoptions)



Typen HtmlSaveOptions avslöjar följande medlemmar:

###  Konstruktörer
| Konstruktör| Beskrivning|
| :- | :- |
| [HtmlSaveOptions()](/cells/sv/python-net/aspose.cells/htmlsaveoptions/__init__/#) | Skapar alternativ för att spara html-fil.|
| [HtmlSaveOptions(format)](/cells/sv/python-net/aspose.cells/htmlsaveoptions/__init__/#SaveFormat) | Skapar alternativ för att spara htm-fil.|


###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [save_format](/cells/sv/python-net/aspose.cells/htmlsaveoptions/save_format) | Hämtar spara filformatet.|
| [clear_data](/cells/sv/python-net/aspose.cells/htmlsaveoptions/clear_data) | Gör arbetsboken tom efter att du har sparat filen.|
| [cached_file_folder](/cells/sv/python-net/aspose.cells/htmlsaveoptions/cached_file_folder) | Den cachade filmappen används för att lagra en del stora data.|
| [validate_merged_areas](/cells/sv/python-net/aspose.cells/htmlsaveoptions/validate_merged_areas) | Anger om sammanslagna celler ska valideras innan filen sparas.|
| [merge_areas](/cells/sv/python-net/aspose.cells/htmlsaveoptions/merge_areas) | Anger om områdena för villkorlig formatering och validering ska slås samman innan filen sparas.|
| [create_directory](/cells/sv/python-net/aspose.cells/htmlsaveoptions/create_directory) | Om sant och katalogen inte finns skapas katalogen automatiskt innan filen sparas.|
| [sort_names](/cells/sv/python-net/aspose.cells/htmlsaveoptions/sort_names) | Anger om du sorterar definierade namn innan filen sparas.|
| [sort_external_names](/cells/sv/python-net/aspose.cells/htmlsaveoptions/sort_external_names) |Anger om externt definierade namn sorteras innan filen sparas.|
| [refresh_chart_cache](/cells/sv/python-net/aspose.cells/htmlsaveoptions/refresh_chart_cache) | Anger om diagramcachedata uppdateras|
| [warning_callback](/cells/sv/python-net/aspose.cells/htmlsaveoptions/warning_callback) | Får eller ställer in varningsåteruppringning.|
| [update_smart_art](/cells/sv/python-net/aspose.cells/htmlsaveoptions/update_smart_art) | Indikerar om inställningen för smart konst uppdateras.<br/> Standardvärdet är falskt.|
| [ignore_invisible_shapes](/cells/sv/python-net/aspose.cells/htmlsaveoptions/ignore_invisible_shapes) |Ange om du exporterar de osynliga formerna|
| [page_title](/cells/sv/python-net/aspose.cells/htmlsaveoptions/page_title) | Titeln på html-sidan.<br/> Endast för att spara till html-ström.|
| [attached_files_directory](/cells/sv/python-net/aspose.cells/htmlsaveoptions/attached_files_directory) | Mappen som de bifogade filerna kommer att sparas i.<br/> Endast för att spara till html-ström.|
| [attached_files_url_prefix](/cells/sv/python-net/aspose.cells/htmlsaveoptions/attached_files_url_prefix) | Ange URL-prefixet för bifogade filer som bild i html-filen.<br/> Endast för att spara till html-ström.|
| [default_font_name](/cells/sv/python-net/aspose.cells/htmlsaveoptions/default_font_name) | Ange standardteckensnittsnamnet för export av html, standardteckensnittet kommer att användas när stiltypsnittet inte finns,<br/>Om den här egenskapen är null kommer Aspose.Cells att använda universella teckensnitt som har samma familj som det ursprungliga teckensnittet,<br/> standardvärdet är null.|
| [worksheet_scalable](/cells/sv/python-net/aspose.cells/htmlsaveoptions/worksheet_scalable) | Indikerar om du zoomar in eller ut html via kalkylbladszoomnivå när du sparar fil till html, standardvärdet är falskt.|
| [is_export_comments](/cells/sv/python-net/aspose.cells/htmlsaveoptions/is_export_comments) | Indikerar om du exporterar kommentarer när du sparar fil till html, standardvärdet är falskt.|
| [export_comments_type](/cells/sv/python-net/aspose.cells/htmlsaveoptions/export_comments_type) | Representerar typ av export av kommentarer till html-filer.|
| [disable_downlevel_revealed_comments](/cells/sv/python-net/aspose.cells/htmlsaveoptions/disable_downlevel_revealed_comments) | Indikerar om inaktivera Downlevel-avslöjade villkorliga kommentarer vid export av fil till html, standardvärdet är false.|
| [is_exp_image_to_temp_dir](/cells/sv/python-net/aspose.cells/htmlsaveoptions/is_exp_image_to_temp_dir) | Anger om bildfiler exporteras till temporär katalog.<br/> Endast för att spara till html-ström.|
| [image_scalable](/cells/sv/python-net/aspose.cells/htmlsaveoptions/image_scalable) | Anger om skalbar enhet används för att beskriva bildens bredd<br/>när du använder skalbar enhet för att beskriva kolumnbredden.<br/> Standardvärdet är sant.|
| [width_scalable](/cells/sv/python-net/aspose.cells/htmlsaveoptions/width_scalable) |Anger om skalbar enhet används för att beskriva kolumnbredden vid export av fil till html.<br/> Standardvärdet är falskt.|
| [export_single_tab](/cells/sv/python-net/aspose.cells/htmlsaveoptions/export_single_tab) | Anger om den enskilda fliken exporteras när filen bara har ett kalkylblad.<br/> Standardvärdet är falskt.|
| [export_images_as_base64](/cells/sv/python-net/aspose.cells/htmlsaveoptions/export_images_as_base64) | Anger om bilder sparas i Base64-format till HTML, MHTML eller EPUB.|
| [export_active_worksheet_only](/cells/sv/python-net/aspose.cells/htmlsaveoptions/export_active_worksheet_only) | Indikerar om hela arbetsboken exporteras till html-fil.|
| [export_print_area_only](/cells/sv/python-net/aspose.cells/htmlsaveoptions/export_print_area_only) | Anger om utskriftsområdet endast exporteras till html-fil. Standardvärdet är falskt.|
| [export_area](/cells/sv/python-net/aspose.cells/htmlsaveoptions/export_area) | Hämtar eller ställer in den exporterande CellArea för det aktuella aktiva arbetsbladet.<br/>Om du ställer in det här attributet kommer utskriftsområdet för det aktuella aktiva arbetsbladet att utelämnas.<br/> Endast det angivna området kommer att exporteras när filen sparas till html.|
| [parse_html_tag_in_cell](/cells/sv/python-net/aspose.cells/htmlsaveoptions/parse_html_tag_in_cell) | Analysera HTML-tagg i cell, som ,som cellvärde eller som HTML-tagg, standard är sant|
| [html_cross_string_type](/cells/sv/python-net/aspose.cells/htmlsaveoptions/html_cross_string_type) | Indikerar om en korscellsträng kommer att visas på samma sätt som MS Excel när du sparar en Excel-fil i html-format.<br/>Som standard är värdet Default, så för korscellsträngar är det liten skillnad mellan html-filerna skapade av Aspose.Cells och MS Excel.<br/> Men prestandan för att skapa stora html-filer, att sätta värdet på Cross skulle vara flera gånger snabbare än att ställa in det till Default eller Fit2Cell.|
| [hidden_col_display_type](/cells/sv/python-net/aspose.cells/htmlsaveoptions/hidden_col_display_type) |Dold kolumn (bredden på denna kolumn är 0) i excel, innan du sparar den i html-format,<br/>om HtmlHiddenColDisplayType är "Remove", skulle den dolda kolumnen inte matas ut,<br/> om värdet är "Dold", skulle kolumnen matas ut, men var dold, standardvärdet är "Dold"|
| [hidden_row_display_type](/cells/sv/python-net/aspose.cells/htmlsaveoptions/hidden_row_display_type) | Dold rad (höjden på denna rad är 0) i excel, innan du sparar den i html-format,<br/>om HtmlHiddenRowDisplayType är "Remove", skulle den dolda raden inte matas ut,<br/> om värdet är "Dold", skulle raden matas ut, men var dold, standardvärdet är "Dold"|
| [encoding](/cells/sv/python-net/aspose.cells/htmlsaveoptions/encoding) | Om inte inställt, använd Encoding.UTF8 som standardkodningstyp.|
| [export_object_listener](/cells/sv/python-net/aspose.cells/htmlsaveoptions/export_object_listener) | Hämtar eller ställer in ExportObjectListener för export av objekt.|
| [file_path_provider](/cells/sv/python-net/aspose.cells/htmlsaveoptions/file_path_provider) | Hämtar eller ställer in IFilePathProvider för export av arbetsblad till html separat.|
| [stream_provider](/cells/sv/python-net/aspose.cells/htmlsaveoptions/stream_provider) | Hämtar eller ställer in IStreamProvider för export av objekt.|
| [image_options](/cells/sv/python-net/aspose.cells/htmlsaveoptions/image_options) | Hämta ImageOrPrintOptions-objektet innan du exporterar|
| [save_as_single_file](/cells/sv/python-net/aspose.cells/htmlsaveoptions/save_as_single_file) | Anger om HTML-filen sparas som en enda fil.<br/> Standardvärdet är falskt.|
| [show_all_sheets](/cells/sv/python-net/aspose.cells/htmlsaveoptions/show_all_sheets) | Anger om alla ark visas när du sparar som en enda html-fil.|
| [export_page_headers](/cells/sv/python-net/aspose.cells/htmlsaveoptions/export_page_headers) | Anger om sidhuvuden exporteras.|
| [export_page_footers](/cells/sv/python-net/aspose.cells/htmlsaveoptions/export_page_footers) | Anger om sidhuvuden exporteras.|
| [export_hidden_worksheet](/cells/sv/python-net/aspose.cells/htmlsaveoptions/export_hidden_worksheet) |Indikerar om det dolda kalkylbladets innehåll exporteras. Standardvärdet är sant.|
| [presentation_preference](/cells/sv/python-net/aspose.cells/htmlsaveoptions/presentation_preference) | Indikerar om html- eller mht-fil är presentationspreferens.<br/>Standardvärdet är falskt.<br/> om du vill få en vackrare presentation, ställ in värdet på sant.|
| [cell_css_prefix](/cells/sv/python-net/aspose.cells/htmlsaveoptions/cell_css_prefix) | Hämtar och ställer in prefixet för css-namnet, standardvärdet är "".|
| [table_css_id](/cells/sv/python-net/aspose.cells/htmlsaveoptions/table_css_id) | Hämtar och ställer in prefixet för typen css-namn som tr,col,td och så vidare, de finns i tabellelementet<br/> som har det specifika TableCssId-attributet. Standardvärdet är "".|
| [is_full_path_link](/cells/sv/python-net/aspose.cells/htmlsaveoptions/is_full_path_link) | Anger om fullständig sökvägslänk används i sheet00x.htm,filelist.xml och tabstrip.htm.<br/> Standardvärdet är falskt.|
| [export_worksheet_css_separately](/cells/sv/python-net/aspose.cells/htmlsaveoptions/export_worksheet_css_separately) | Anger om kalkylbladets css exporteras separat. Standardvärdet är falskt.|
| [export_similar_border_style](/cells/sv/python-net/aspose.cells/htmlsaveoptions/export_similar_border_style) | Anger om liknande kantstil exporteras när kantstilen inte stöds av webbläsare.<br/>Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet.<br/> Standardvärdet är falskt.|
| [merge_empty_td_forcely](/cells/sv/python-net/aspose.cells/htmlsaveoptions/merge_empty_td_forcely) | Indikerar om sammanslagning av tomt TD-element tvångsmässigt vid export av fil till html.<br/> Storleken på html-filen kommer att minskas avsevärt efter att värdet ställts in på sant. Standardvärdet är falskt.<br/> Om du vill importera html-filen till Excel eller exportera perfekta rutnätslinjer när du sparar filen till html,<br/> behåll standardvärdet.|
| [export_cell_coordinate](/cells/sv/python-net/aspose.cells/htmlsaveoptions/export_cell_coordinate) |Anger om excel-koordinater för icke-tomma celler exporteras när filen sparas till html. Standardvärdet är falskt.<br/> Om du vill importera utdata-html till excel, behåll standardvärdet.|
| [export_extra_headings](/cells/sv/python-net/aspose.cells/htmlsaveoptions/export_extra_headings) | Anger om extra rubriker exporteras när textens längd är längre än maxvisningskolumnen.<br/> Standardvärdet är falskt. Om du vill importera html-filen till Excel, behåll standardvärdet.|
| [export_headings](/cells/sv/python-net/aspose.cells/htmlsaveoptions/export_headings) | Anger om arkets rad- och kolumnrubriker exporteras när du sparar till HTML-filer.|
| [export_row_column_headings](/cells/sv/python-net/aspose.cells/htmlsaveoptions/export_row_column_headings) | Anger om arkets rad- och kolumnrubriker exporteras när du sparar till HTML-filer.|
| [export_formula](/cells/sv/python-net/aspose.cells/htmlsaveoptions/export_formula) | Anger om formeln exporteras när filen sparas till html. Standardvärdet är sant.<br/> Om du vill importera utdata-html till excel, behåll standardvärdet.|
| [add_tooltip_text](/cells/sv/python-net/aspose.cells/htmlsaveoptions/add_tooltip_text) | Anger om man lägger till verktygstipstext när data inte kan visas helt.<br/> Standardvärdet är falskt.|
| [export_grid_lines](/cells/sv/python-net/aspose.cells/htmlsaveoptions/export_grid_lines) | Anger om rutnätslinjerna exporteras. Standardvärdet är falskt.|
| [export_bogus_row_data](/cells/sv/python-net/aspose.cells/htmlsaveoptions/export_bogus_row_data) | Anger om falsk data på nedre raden exporteras. Standardvärdet är true.Om du vill importera html- eller mht-filen<br/> för att excel, vänligen behåll standardvärdet.|
| [exclude_unused_styles](/cells/sv/python-net/aspose.cells/htmlsaveoptions/exclude_unused_styles) | Anger om oanvända stilar utesluts.<br/>För de genererade html-filerna kan filstorleken bli mindre om du utesluter oanvända formatmallar<br/>utan att påverka de visuella effekterna. Så standardvärdet för den här egenskapen är sant.<br/>Om användaren behöver behålla alla stilar i arbetsboken för den genererade HTML-koden (som scenariot för den användaren<br/>behöver återställa arbetsboken från den genererade HTML-koden senare), vänligen ställ in den här egenskapen som falsk.|
| [export_document_properties](/cells/sv/python-net/aspose.cells/htmlsaveoptions/export_document_properties) | Anger om dokumentegenskaper exporteras. Standardvärdet är sant. Om du vill importera<br/> html- eller mht-filen för att excel, behåll standardvärdet.|
| [export_worksheet_properties](/cells/sv/python-net/aspose.cells/htmlsaveoptions/export_worksheet_properties) | Anger om kalkylbladsegenskaper exporteras. Standardvärdet är sant. Om du vill importera<br/> html- eller mht-filen för att excel, behåll standardvärdet.|
| [export_workbook_properties](/cells/sv/python-net/aspose.cells/htmlsaveoptions/export_workbook_properties) | Anger om arbetsboksegenskaper exporteras. Standardvärdet är sant. Om du vill importera<br/> html- eller mht-filen för att excel, behåll standardvärdet.|
| [export_frame_scripts_and_properties](/cells/sv/python-net/aspose.cells/htmlsaveoptions/export_frame_scripts_and_properties) | Anger om ramskript och dokumentegenskaper exporteras. Standardvärdet är true.Om du vill importera html- eller mht-filen<br/> för att excel, vänligen behåll standardvärdet.|
| [export_data_options](/cells/sv/python-net/aspose.cells/htmlsaveoptions/export_data_options) | Indikerar regeln för export av html-fildata. Standardvärdet är Alla.|
| [link_target_type](/cells/sv/python-net/aspose.cells/htmlsaveoptions/link_target_type) | Anger typen av målattribut i<a> länk, Standardvärdet är HtmlLinkTargetType.Parent.|



###  Se även
* modul [aspose.cells](..)
* klass [HtmlSaveOptions](/cells/sv/python-net/aspose.cells/htmlsaveoptions)
* klass [SaveOptions](/cells/sv/python-net/aspose.cells/saveoptions)
