##GridJsWorkbook class
## GridJsWorkbook class
Represents the main entry class for GridJs
The GridJsWorkbook type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/__init__/#) | Constructs a new instance of GridJsWorkbook |
### Properties
| Property | Description |
| :- | :- |
| [settings](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/settings) | Represents the workbook settings. |
| [cache_imp](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/cache_imp) | Custom  implemention for cache storage,If you want to store cache in stream way ,you  need to set and implement it. |
| [calculate_engine](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/calculate_engine) | Custom  implemention for calculation engine ,If you want to do custom calculation, you  need to set and implement it. |
### Methods
| Method | Description |
| :- | :- |
| [import_excel_file](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/import_excel_file/#str-str-str) | Imports the excel file from file path and open password. |
| [import_excel_file](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/import_excel_file/#str-str) | Imports the excel file from the file path. |
| [import_excel_file](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/import_excel_file/#str) | Imports the excel file from the file path. |
| [import_excel_file](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/import_excel_file/#str-io.RawIOBase-aspose.cellsgridjs.GridLoadFormat-str) | Imports the excel file from  file stream with load format and open password. |
| [import_excel_file](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/import_excel_file/#str-io.RawIOBase-aspose.cellsgridjs.GridLoadFormat) | Imports the excel file from file stream. |
| [import_excel_file](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/import_excel_file/#io.RawIOBase-aspose.cellsgridjs.GridLoadFormat-str) | Imports the excel file from file stream with load format and open password. |
| [import_excel_file](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/import_excel_file/#io.RawIOBase-aspose.cellsgridjs.GridLoadFormat) | Imports the excel file from file stream with load format. |
| [export_to_json](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/export_to_json/#str) | Gets JSON format string from memory data with the specified filename. |
| [export_to_json](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/export_to_json/#) | Gets JSON format string of the default empty spreadsheet file. |
| [save_to_excel_file](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/save_to_excel_file/#io.RawIOBase) | Saves the memory data to the sream, baseed on the origin file format. |
| [save_to_excel_file](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/save_to_excel_file/#str) | Saves the memory data to the file path,if the file has extension ,save format is baseed on the file extension . |
| [save_to_pdf](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/save_to_pdf/#str) | Saves the memory data to the file path,the save format is pdf. |
| [save_to_pdf](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/save_to_pdf/#io.RawIOBase) | Saves the memory data to the sream,the save format is pdf. |
| [save_to_xlsx](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/save_to_xlsx/#str) | Saves the memory data to the file path,the save format is xlsx. |
| [save_to_xlsx](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/save_to_xlsx/#io.RawIOBase) | Saves the memory data to the sream,the save format is xlsx. |
| [save_to_html](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/save_to_html/#str) | Saves the memory data to the file path,the save format is html. |
| [save_to_html](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/save_to_html/#io.RawIOBase) | Saves the memory data to the sream,the save format is html |
| [get_json_str_by_uid](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/get_json_str_by_uid/#str-str) | Gets the JSON format string from the file cache by the specified unique id. |
| [get_uid_for_file](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/get_uid_for_file/#str) | Gets unique id for the file cache. |
| [import_excel_file_from_json](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/import_excel_file_from_json/#str) | Imports the excel file from JSON format string. |
| [merge_excel_file_from_json](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/merge_excel_file_from_json/#str-str) | Applies a batch update to the memory data. |
| [save_to_cache_with_file_name](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/save_to_cache_with_file_name/#str-str-str) | Saves the memory data to the cache file with the specified filename and also set the open password, the save format is baseed on the file extension of the filename  . |
| [get_image_stream](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/get_image_stream/#str-str) | Get Stream of image from memory data. |
| [get_ole](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/get_ole/#str-str-int-any) | Gets the byte array data of the  embedded ole object . |
| [update_cell](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/update_cell/#str-str) | Applies the update operation. |
| [insert_image](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/insert_image/#str-str-io.RawIOBase-str) | Inserts image in the worksheet from file stream or the URL,(either the file stream or the URL shall be provided)<br/>or /cells/<br/>Inserts sh/cells/n the p.type is one of AutoShapeType |
| [copy_image_or_shape](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/copy_image_or_shape/#str-str) | Copys image or shape. |
| [error_json](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/error_json/#str) | Gets the error message string in JSON format. |
| [get_grid_load_format](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/get_grid_load_format/#str) | Gets the load format by file extension |
| [get_image_url](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/get_image_url/#str-str-str) | Gets the image URL. |
| [set_image_url_base](/cells/python-net/aspose.cellsgridjs/gridjsworkbook/set_image_url_base/#str) |  |
### See Also
* module [`aspose.cellsgridjs`](..)
