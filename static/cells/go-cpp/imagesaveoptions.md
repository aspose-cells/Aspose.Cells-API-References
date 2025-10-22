##ImageSaveOptions Class
'ImageSaveOptions class. Encapsulates the object that represents imagesaveoptions in Go.'
## ImageSaveOptions class
Represents image save options.For advanced usage, please use <see cref="WorkbookRender"/> or <see cref="SheetRender"/>.
```go
type ImageSaveOptions struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewImageSaveOptions](./newimagesaveoptions/) | Creates the options for saving image file. |
|[NewImageSaveOptions_SaveFormat](./newimagesaveoptions_saveformat/) | Creates the options for saving image file. |
|[NewImageSaveOptions_SaveOptions](./newimagesaveoptions_saveoptions/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetImageOrPrintOptions](./getimageorprintoptions/) | Additional image creation options. |
|[GetSaveFormat](./getsaveformat/) | Gets the save file format. |
|[GetClearData](./getcleardata/) | Make the workbook empty after saving the file. |
|[SetClearData](./setcleardata/) | Make the workbook empty after saving the file. |
|[GetCachedFileFolder](./getcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
|[SetCachedFileFolder](./setcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
|[GetValidateMergedAreas](./getvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
|[SetValidateMergedAreas](./setvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
|[GetMergeAreas](./getmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
|[SetMergeAreas](./setmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
|[GetCreateDirectory](./getcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
|[SetCreateDirectory](./setcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
|[GetSortNames](./getsortnames/) | Indicates whether sorting defined names before saving file. |
|[SetSortNames](./setsortnames/) | Indicates whether sorting defined names before saving file. |
|[GetSortExternalNames](./getsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
|[SetSortExternalNames](./setsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
|[GetRefreshChartCache](./getrefreshchartcache/) | Indicates whether refreshing chart cache data |
|[SetRefreshChartCache](./setrefreshchartcache/) | Indicates whether refreshing chart cache data |
|[GetCheckExcelRestriction](./getcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects.For example, excel does not allow inputting string value longer than 32K.When you input a value longer than 32K, it will be truncated. |
|[SetCheckExcelRestriction](./setcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects.For example, excel does not allow inputting string value longer than 32K.When you input a value longer than 32K, it will be truncated. |
|[GetUpdateSmartArt](./getupdatesmartart/) | Indicates whether updating smart art setting.The default value is false. |
|[SetUpdateSmartArt](./setupdatesmartart/) | Indicates whether updating smart art setting.The default value is false. |
|[GetEncryptDocumentProperties](./getencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file.The default value is true. |
|[SetEncryptDocumentProperties](./setencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file.The default value is true. |
