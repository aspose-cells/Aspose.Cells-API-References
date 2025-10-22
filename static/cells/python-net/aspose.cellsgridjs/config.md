##Config class
## Config class
Represents all the settings for GridJs
The Config type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/cells/python-net/aspose.cellsgridjs/config/__init__/#) | Constructs a new instance of Config |
### Properties
| Property | Description |
| :- | :- |
| [save_html_as_zip](/cells/python-net/aspose.cellsgridjs/config/save_html_as_zip) | Sets/Gets  whether to save html file as zip archive,the default is false. |
| [same_image_detecting](/cells/python-net/aspose.cellsgridjs/config/same_image_detecting) | Sets/Gets  whether to check if picture has same source,the default is true<br/>the default value is true. |
| [auto_optimize_for_large_cells](/cells/python-net/aspose.cellsgridjs/config/auto_optimize_for_large_cells) | Sets/Gets  whether to automatically optimize the load performance for worksheet with large cells<br/>ignore some style /borders to reduce the load  time <br/>the default value is true. |
| [islimit_shape_or_image](/cells/python-net/aspose.cellsgridjs/config/islimit_shape_or_image) | Sets/Gets  whether to limit the total display shape/image count inside one worksheet ,if set to true, <br/>GridJs will limit the total display shape/image size inside one worksheet  to MaxShapeOrImageCount <br/>the default value is true. |
| [max_shape_or_image_count](/cells/python-net/aspose.cellsgridjs/config/max_shape_or_image_count) | Sets/Gets the total display shape/image count inside the active sheet,it will take affec when IslimitShapes=true. <br/>the default value is 100. |
| [max_total_shape_or_image_count](/cells/python-net/aspose.cellsgridjs/config/max_total_shape_or_image_count) | Sets/Gets the total display shape/image count inside the whole workbook,it will take affec when IslimitShapes=true. <br/>the default value is 300. |
| [max_shape_or_image_width_or_height](/cells/python-net/aspose.cellsgridjs/config/max_shape_or_image_width_or_height) | Sets/Gets the  max width or height for a shape/image ,GridJs will ignore the shape/image with the width or height larger than this, it will take affec when IslimitShapes=true. <br/>the default value is 10000. |
| [max_pdf_save_seconds](/cells/python-net/aspose.cellsgridjs/config/max_pdf_save_seconds) | Sets/Gets the max timed out seconds when save to pdf. <br/>the default value is 10. |
| [ignore_empty_content](/cells/python-net/aspose.cellsgridjs/config/ignore_empty_content) | Sets/Gets whether to show  the max range which includes data ,style, merged cells and shapes. <br/>if the last row or column contains cells with  no value and formula but has custom style <br/>then we will not show this row/column when this vlaue is true。<br/>the default value is true . |
| [use_print_area](/cells/python-net/aspose.cellsgridjs/config/use_print_area) | Sets/Gets whether to use PageSetup.PrintArea for the UI display range when the worksheet has PageSetup setting for PrintArea. <br/>the default value is false . |
| [load_time_out](/cells/python-net/aspose.cellsgridjs/config/load_time_out) | Sets/Gets a timeout interrupt in milliseconds in loading file, when the cost time period of loading file  is longer than the expectation，it will raise exception. <br/>the default value is -1,which means no timeout interrupt is set . |
| [show_chart_sheet](/cells/python-net/aspose.cellsgridjs/config/show_chart_sheet) | Sets/Gets whether to show chart worksheet. <br/>the default value is false . |
| [page_size](/cells/python-net/aspose.cellsgridjs/config/page_size) | Sets/Gets whether to do pagination <br/>GridJs will limit the row size based on the PageSize,if PageSize is -1,it will not do pagination <br/>the default value is -1 |
| [empty_sheet_max_row](/cells/python-net/aspose.cellsgridjs/config/empty_sheet_max_row) | Sets/Gets default max row for an empty worksheet. <br/>the default value is 12. |
| [empty_sheet_max_col](/cells/python-net/aspose.cellsgridjs/config/empty_sheet_max_col) | Sets/Gets default max column for an empty worksheet. <br/>the default value is 15. |
| [picture_cache_directory](/cells/python-net/aspose.cellsgridjs/config/picture_cache_directory) | Sets/Gets the cache directory for pictures.(this will take affect when GridJsWorkbook.CacheImp is null) <br/>the default path will be "_piccache" inside the FileCacheDirectory. |
| [file_cache_directory](/cells/python-net/aspose.cellsgridjs/config/file_cache_directory) | Sets/Gets the cache directory for spreadsheet file. <br/>We need to set it to a specific path before we use GridJs. |
### Methods
| Method | Description |
| :- | :- |
| [set_license](/cells/python-net/aspose.cellsgridjs/config/set_license/#str) |  |
| [set_license](/cells/python-net/aspose.cellsgridjs/config/set_license/#io.RawIOBase) | Licenses the component. |
| [set_font_folder](/cells/python-net/aspose.cellsgridjs/config/set_font_folder/#str-bool) | Sets the fonts folder |
| [set_font_folders](/cells/python-net/aspose.cellsgridjs/config/set_font_folders/#list-bool) | Sets the fonts folders |
### See Also
* module [`aspose.cellsgridjs`](..)
