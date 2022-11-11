---
title: ImageOrPrintOptions
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 40
url: /cells/python-net/aspose.cells.rendering/imageorprintoptions/
---

## ImageOrPrintOptions class

Allows to specify options when rendering worksheet to images, printing worksheet or rendering chart to image.

The ImageOrPrintOptions type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|ImageOrPrintOptions()|Initializes a new instance of the ImageOrPrintOptions class|
## Properties
| Name | Description |
| :- | :- |
|save_format|Gets or sets the output file format type<br/>            Support Tiff/XPS|
|print_with_status_dialog|If PrintWithStatusDialog = true , there will be a dialog that shows current print status.<br/>            else no such dialog will show.|
|horizontal_resolution|Gets or sets the horizontal resolution for generated images, in dots per inch.<br/>            Applies generating image method except Emf format images.|
|vertical_resolution|Gets or sets the vertical  resolution for generated images, in dots per inch.<br/>            Applies generating image method except Emf format image.|
|tiff_compression|Gets or sets the type of compression to apply only when saving pages to the|
|tiff_color_depth|Gets or sets bit depth to apply only when saving pages to the|
|printing_page|Indicates which pages will not be printed.|
|quality|Gets or sets a value determining the quality of the generated  images<br/>            to apply only when saving pages to the|
|image_type|Gets or sets the format of the generated images.<br/>            default value: PNG.|
|is_cell_auto_fit|Indicates whether the width and height of the cells is automatically fitted by cell value. <br/>            The default value is false.|
|one_page_per_sheet|If OnePagePerSheet is true , all content of one sheet will output to only one page in result. <br/>            The paper size of pagesetup will be invalid, and the other settings of pagesetup <br/>            will still take effect.|
|all_columns_in_one_page_per_sheet|If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. <br/>            The width of paper size of pagesetup will be invalid, and the other settings of pagesetup <br/>            will still take effect.|
|draw_object_event_handler|Implements this interface to get DrawObject and Bound when rendering.|
|chart_image_type|Indicate the chart imagetype when converting.<br/>            default value: PNG.|
|embeded_image_name_in_svg|Indicate the filename of embedded image in svg. <br/>            This should be full path with directory like "c:\\xpsEmbedded"|
|svg_fit_to_view_port|if this property is true, the generated svg will fit to view port.|
|only_area|If this property is true , one Area will be output, and no scale will take effect.|
|text_rendering_hint|Specifies the quality of text rendering.<br/>            The default value is TextRenderingHint.SystemDefault|
|smoothing_mode|Specifies whether smoothing (antialiasing) is applied to lines and curves and the edges of filled areas.<br/>            The default value is SmoothingMode.None|
|transparent|Indicates if the background of generated image should be transparent.|
|pixel_format|Gets or sets the pixel format for the generated images.|
|warning_callback|Gets or sets warning callback.|
|page_saving_callback|Control/Indicate progress of page saving process.|
|is_font_substitution_char_granularity|Indicates whether to only substitute the font of character when the cell font is not compatibility for it.|
|page_index|Gets or sets the 0-based index of the first page to save.|
|page_count|Gets or sets the number of pages to save.|
|is_optimized|Indicates whether to optimize the output elements.|
|default_font|When characters in the Excel are Unicode and not be set with correct font in cell style,<br/>            They may appear as block in pdf,image.<br/>            Set the DefaultFont such as MingLiu or MS Gothic to show these characters.<br/>            If this property is not set, Aspose.Cells will use system default font to show these unicode characters.|
|check_workbook_default_font|When characters in the Excel are Unicode and not be set with correct font in cell style,<br/>            They may appear as block in pdf,image.<br/>            Set this to true to try to use workbook's default font to show these characters first.|
|output_blank_page_when_nothing_to_print|Indicates whether to output a blank page when there is nothing to print.|
|gridline_type|Gets or sets gridline type.|
|text_cross_type|Gets or sets displaying text type when the text width is larger than cell width.|
|emf_type|Gets or sets an EmfType that specifies the format of the Metafile..|
|default_edit_language|Gets or sets default edit language.|
|sheet_set|Gets or sets the sheets to render. Default is all visible sheets in the workbook: [visible](/cells/python-net/aspose.cells.rendering/sheetset/).|
## Methods
| Name | Description |
| :- | :- |
|set_desired_size(desired_width, desired_height)|Sets desired width and height of image.|

### See Also

* namespace [aspose.cells.rendering](/cells/python-net/aspose.cells.rendering/)
* assembly [Aspose.Cells](/cells/python-net/)

