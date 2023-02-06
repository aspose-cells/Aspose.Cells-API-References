---
title: PdfSaveOptions class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 1180
url: /python-net/aspose.cells/pdfsaveoptions/
is_root: false
---

## PdfSaveOptions class

Represents the options for saving pdf file.



**Inheritance:** [PdfSaveOptions](/cells/python-net/aspose.cells/pdfsaveoptions) → 
[PaginatedSaveOptions](/cells/python-net/aspose.cells/paginatedsaveoptions) → 
[SaveOptions](/cells/python-net/aspose.cells/saveoptions)



The PdfSaveOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [PdfSaveOptions()](/cells/python-net/aspose.cells/pdfsaveoptions/__init__/#) | Creates the options for saving pdf file. |


### Properties
| Property | Description |
| :- | :- |
| [save_format](/cells/python-net/aspose.cells/pdfsaveoptions/save_format) | Gets the save file format. |
| [clear_data](/cells/python-net/aspose.cells/pdfsaveoptions/clear_data) | Make the workbook empty after saving the file. |
| [cached_file_folder](/cells/python-net/aspose.cells/pdfsaveoptions/cached_file_folder) | The cached file folder is used to store some large data. |
| [validate_merged_areas](/cells/python-net/aspose.cells/pdfsaveoptions/validate_merged_areas) | Indicates whether validate merged cells before saving the file. |
| [merge_areas](/cells/python-net/aspose.cells/pdfsaveoptions/merge_areas) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [create_directory](/cells/python-net/aspose.cells/pdfsaveoptions/create_directory) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [sort_names](/cells/python-net/aspose.cells/pdfsaveoptions/sort_names) | Indicates whether sorting defined names before saving file. |
| [sort_external_names](/cells/python-net/aspose.cells/pdfsaveoptions/sort_external_names) | Indicates whether sorting external defined names before saving file. |
| [refresh_chart_cache](/cells/python-net/aspose.cells/pdfsaveoptions/refresh_chart_cache) | Indicates whether refreshing chart cache data |
| [warning_callback](/cells/python-net/aspose.cells/pdfsaveoptions/warning_callback) | Gets or sets warning callback. |
| [update_smart_art](/cells/python-net/aspose.cells/pdfsaveoptions/update_smart_art) | Indicates whether updating smart art setting.<br/>The default value is false. |
| [default_font](/cells/python-net/aspose.cells/pdfsaveoptions/default_font) | When characters in the Excel are Unicode and not be set with correct font in cell style,<br/>They may appear as block in pdf,image.<br/>Set the DefaultFont such as MingLiu or MS Gothic to show these characters.<br/>If this property is not set, Aspose.Cells will use system default font to show these unicode characters. |
| [check_workbook_default_font](/cells/python-net/aspose.cells/pdfsaveoptions/check_workbook_default_font) | When characters in the Excel are Unicode and not be set with correct font in cell style,<br/>They may appear as block in pdf,image.<br/>Set this to true to try to use workbook's default font to show these characters first. |
| [check_font_compatibility](/cells/python-net/aspose.cells/pdfsaveoptions/check_font_compatibility) | Indicates whether to check font compatibility for every character in text. |
| [is_font_substitution_char_granularity](/cells/python-net/aspose.cells/pdfsaveoptions/is_font_substitution_char_granularity) | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [one_page_per_sheet](/cells/python-net/aspose.cells/pdfsaveoptions/one_page_per_sheet) | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. <br/>The paper size of pagesetup will be invalid, and the other settings of pagesetup <br/>will still take effect. |
| [all_columns_in_one_page_per_sheet](/cells/python-net/aspose.cells/pdfsaveoptions/all_columns_in_one_page_per_sheet) | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. <br/>The width of paper size of pagesetup will be ignored, and the other settings of pagesetup <br/>will still take effect. |
| [ignore_error](/cells/python-net/aspose.cells/pdfsaveoptions/ignore_error) | Indicates if you need to hide the error while rendering.<br/>The error can be error in shape, image, chart rendering, etc. |
| [output_blank_page_when_nothing_to_print](/cells/python-net/aspose.cells/pdfsaveoptions/output_blank_page_when_nothing_to_print) | Indicates whether to output a blank page when there is nothing to print. |
| [page_index](/cells/python-net/aspose.cells/pdfsaveoptions/page_index) | Gets or sets the 0-based index of the first page to save. |
| [page_count](/cells/python-net/aspose.cells/pdfsaveoptions/page_count) | Gets or sets the number of pages to save. |
| [printing_page_type](/cells/python-net/aspose.cells/pdfsaveoptions/printing_page_type) | Indicates which pages will not be printed. |
| [gridline_type](/cells/python-net/aspose.cells/pdfsaveoptions/gridline_type) | Gets or sets gridline type. |
| [text_cross_type](/cells/python-net/aspose.cells/pdfsaveoptions/text_cross_type) | Gets or sets displaying text type when the text width is larger than cell width. |
| [default_edit_language](/cells/python-net/aspose.cells/pdfsaveoptions/default_edit_language) | Gets or sets default edit language. |
| [sheet_set](/cells/python-net/aspose.cells/pdfsaveoptions/sheet_set) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: [SheetSet.visible](/cells/python-net/aspose.cells.rendering/sheetset#visible). |
| [draw_object_event_handler](/cells/python-net/aspose.cells/pdfsaveoptions/draw_object_event_handler) | Implements this interface to get DrawObject and Bound when rendering. |
| [page_saving_callback](/cells/python-net/aspose.cells/pdfsaveoptions/page_saving_callback) | Control/Indicate progress of page saving process. |
| [embed_standard_windows_fonts](/cells/python-net/aspose.cells/pdfsaveoptions/embed_standard_windows_fonts) | True to embed true type fonts. <br/>Affects only ASCII characters 32-127.<br/>Fonts for character codes greater than 127 are always embedded.<br/>Fonts are always embedded for PDF/A-1a, PDF/A-1b standard.<br/>Default is true. |
| [bookmark](/cells/python-net/aspose.cells/pdfsaveoptions/bookmark) | Gets and sets the [PdfBookmarkEntry](/cells/python-net/aspose.cells.rendering/pdfbookmarkentry) object. |
| [compliance](/cells/python-net/aspose.cells/pdfsaveoptions/compliance) | Workbook converts to pdf will according to PdfCompliance in this property. |
| [security_options](/cells/python-net/aspose.cells/pdfsaveoptions/security_options) | Set this options, when security is need in xls2pdf result. |
| [image_type](/cells/python-net/aspose.cells/pdfsaveoptions/image_type) | Represents the image type when converting the chart and shape . |
| [calculate_formula](/cells/python-net/aspose.cells/pdfsaveoptions/calculate_formula) | Indicates whether to calculate formulas before saving pdf file. |
| [pdf_compression](/cells/python-net/aspose.cells/pdfsaveoptions/pdf_compression) | Indicate the compression algorithm |
| [created_time](/cells/python-net/aspose.cells/pdfsaveoptions/created_time) | Gets and sets the time of generating the pdf document. |
| [producer](/cells/python-net/aspose.cells/pdfsaveoptions/producer) | Gets and sets producer of generated pdf document. |
| [optimization_type](/cells/python-net/aspose.cells/pdfsaveoptions/optimization_type) | Gets and sets pdf optimization type. |
| [custom_properties_export](/cells/python-net/aspose.cells/pdfsaveoptions/custom_properties_export) | Gets or sets a value determining the way [CustomDocumentPropertyCollection](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection) are exported to PDF file. Default value is None. |
| [export_document_structure](/cells/python-net/aspose.cells/pdfsaveoptions/export_document_structure) | Indicates whether to export document structure. |
| [emf_render_setting](/cells/python-net/aspose.cells/pdfsaveoptions/emf_render_setting) | Setting for rendering Emf metafile. |
| [display_doc_title](/cells/python-net/aspose.cells/pdfsaveoptions/display_doc_title) | Indicates whether the window's title bar should display the document title. |
| [font_encoding](/cells/python-net/aspose.cells/pdfsaveoptions/font_encoding) | Gets or sets embedded font encoding in pdf. |


### Methods
| Method | Description |
| :- | :- |
| [set_image_resample(desired_ppi, jpeg_quality)](/cells/python-net/aspose.cells/pdfsaveoptions/set_image_resample/#int-int) | Sets desired PPI(pixels per inch) of resample images and jpeg quality.  <br/>All images will be converted to JPEG with the specified quality setting, <br/>and images that are greater than the specified PPI (pixels per inch) will be resampled. |



### See Also
* module [aspose.cells](..)
* class [CustomDocumentPropertyCollection](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection)
* class [PaginatedSaveOptions](/cells/python-net/aspose.cells/paginatedsaveoptions)
* class [PdfBookmarkEntry](/cells/python-net/aspose.cells.rendering/pdfbookmarkentry)
* class [PdfSaveOptions](/cells/python-net/aspose.cells/pdfsaveoptions)
* class [SaveOptions](/cells/python-net/aspose.cells/saveoptions)
