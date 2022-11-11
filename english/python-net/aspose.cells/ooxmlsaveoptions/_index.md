---
title: OoxmlSaveOptions
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 1120
url: /python-net/aspose.cells/ooxmlsaveoptions/
---

## OoxmlSaveOptions class

Represents the options of saving office open xml file.

The OoxmlSaveOptions type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|OoxmlSaveOptions()|Creates the options for saving office open xml file.|
|OoxmlSaveOptions(save_format)|Initializes a new instance of the OoxmlSaveOptions class|
## Properties
| Name | Description |
| :- | :- |
|save_format|Gets the save file format.|
|clear_data|Make the workbook empty after saving the file.|
|cached_file_folder|The cached file folder is used to store some large data.|
|validate_merged_areas|Indicates whether validate merged cells before saving the file.|
|merge_areas|Indicates whether merge the areas of conditional formatting and validation before saving the file.|
|create_directory|If true and the directory does not exist, the directory will be automatically created before saving the file.|
|sort_names|Indicates whether sorting defined names before saving file.|
|sort_external_names|Indicates whether sorting external defined names before saving file.|
|refresh_chart_cache|Indicates whether refreshing chart cache data|
|warning_callback|Gets or sets warning callback.|
|update_smart_art|Indicates whether updating smart art setting.<br/>            The default value is false.|
|export_cell_name|Indicates if export cell name to Excel2007 .xlsx (.xlsm, .xltx, .xltm) file. <br/>            If the output file may be accessed by SQL Server DTS, this value must be true.<br/>            Setting the value to false will highly increase the performance and reduce the file size when creating large file.<br/>            Default value is true.|
|light_cells_data_provider|The Data provider to provide cells data for saving workbook in light mode.|
|update_zoom|Indicates whether update scaling factor before saving the file <br/>            if the PageSetup.FitToPagesWide and PageSetup.FitToPagesTall properties control how the worksheet is scaled.|
|enable_zip64|Always use ZIP64 extensions when writing zip archives, even when unnecessary.|
|embed_ooxml_as_ole_object|Indicates whether embedding Ooxml files of OleObject as ole object.|
|compression_type|Gets and sets the compression type for ooxml file.|

### See Also

* namespace [aspose.cells](/python-net/aspose.cells/)
* assembly [Aspose.Cells](/python-net/)

