---
title: PdfSaveOptions
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 1180
url: /python-net/aspose.cells/pdfsaveoptions/
---

## PdfSaveOptions class

Represents the options for saving pdf file.

The PdfSaveOptions type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|PdfSaveOptions()|Creates the options for saving pdf file.|
## Properties
| Name | Description |
| :- | :- |
|save_format|  |
|clear_data|  |
|cached_file_folder|  |
|validate_merged_areas|  |
|merge_areas|  |
|create_directory|  |
|sort_names|  |
|sort_external_names|  |
|refresh_chart_cache|  |
|warning_callback|  |
|update_smart_art|  |
|default_font|When characters in the Excel are Unicode and not be set with correct font in cell style,<br/>            They may appear as block in pdf,image.<br/>            Set the DefaultFont such as MingLiu or MS Gothic to show these characters.<br/>            If this property is not set, Aspose.Cells will use system default font to show these unicode characters.|
|check_workbook_default_font|When characters in the Excel are Unicode and not be set with correct font in cell style,<br/>            They may appear as block in pdf,image.<br/>            Set this to true to try to use workbook's default font to show these characters first.|
|check_font_compatibility|Indicates whether to check font compatibility for every character in text.|
|is_font_substitution_char_granularity|Indicates whether to only substitute the font of character when the cell font is not compatibility for it.|
|one_page_per_sheet|If OnePagePerSheet is true , all content of one sheet will output to only one page in result. <br/>            The paper size of pagesetup will be invalid, and the other settings of pagesetup <br/>            will still take effect.|
|all_columns_in_one_page_per_sheet|If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. <br/>            The width of paper size of pagesetup will be ignored, and the other settings of pagesetup <br/>            will still take effect.|
|ignore_error|Indicates if you need to hide the error while rendering.<br/>            The error can be error in shape, image, chart rendering, etc.|
|output_blank_page_when_nothing_to_print|Indicates whether to output a blank page when there is nothing to print.|
|page_index|Gets or sets the 0-based index of the first page to save.|
|page_count|Gets or sets the number of pages to save.|
|printing_page_type|Indicates which pages will not be printed.|
|gridline_type|Gets or sets gridline type.|
|text_cross_type|Gets or sets displaying text type when the text width is larger than cell width.|
|default_edit_language|Gets or sets default edit language.|
|sheet_set|Gets or sets the sheets to render. Default is all visible sheets in the workbook: [visible](/cells/python-net/aspose.cells.rendering/sheetset/).|
|draw_object_event_handler|Implements this interface to get DrawObject and Bound when rendering.|
|page_saving_callback|Control/Indicate progress of page saving process.|
|embed_standard_windows_fonts|True to embed true type fonts. <br/>            Affects only ASCII characters 32-127.<br/>            Fonts for character codes greater than 127 are always embedded.<br/>            Fonts are always embedded for PDF/A-1a, PDF/A-1b standard.<br/>            Default is true.|
|bookmark|Gets and sets the|
|compliance|Workbook converts to pdf will according to PdfCompliance in this property.|
|security_options|Set this options, when security is need in xls2pdf result.|
|image_type|Represents the image type when converting the chart and shape .|
|calculate_formula|Indicates whether to calculate formulas before saving pdf file.|
|pdf_compression|Indicate the compression algorithm|
|created_time|Gets and sets the time of generating the pdf document.|
|producer|Gets and sets producer of generated pdf document.|
|optimization_type|Gets and sets pdf optimization type.|
|custom_properties_export|Gets or sets a value determining the way [CustomDocumentPropertyCollection](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection/) are exported to PDF file. Default value is None.|
|export_document_structure|Indicates whether to export document structure.|
|emf_render_setting|Setting for rendering Emf metafile.|
|display_doc_title|Indicates whether the window's title bar should display the document title.|
|font_encoding|Gets or sets embedded font encoding in pdf.|
## Methods
| Name | Description |
| :- | :- |
|set_image_resample(desired_ppi, jpeg_quality)|Sets desired PPI(pixels per inch) of resample images and jpeg quality.  <br/>            All images will be converted to JPEG with the specified quality setting, <br/>            and images that are greater than the specified PPI (pixels per inch) will be resampled.|

### See Also

* namespace [aspose.cells](/cells/python-net/aspose.cells/)
* assembly [Aspose.Cells](/cells/python-net/)

