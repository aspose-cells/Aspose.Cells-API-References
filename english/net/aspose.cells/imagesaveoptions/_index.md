---
title: Class ImageSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ImageSaveOptions class. Represents image save options. For advanced usage please use WorkbookRender or SheetRender
type: docs
url: /net/aspose.cells/imagesaveoptions/
---
## ImageSaveOptions class

Represents image save options. For advanced usage, please use [`WorkbookRender`](../../aspose.cells.rendering/workbookrender/) or [`SheetRender`](../../aspose.cells.rendering/sheetrender/).

```csharp
public class ImageSaveOptions : SaveOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions/#constructor)() | Creates the options for saving image file. |
| [ImageSaveOptions](imagesaveoptions/#constructor_1)(SaveFormat) | Creates the options for saving image file. |

## Properties

| Name | Description |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | The cached file folder is used to store some large data.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Make the workbook empty after saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | If true and the directory does not exist, the directory will be automatically created before saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indicates whether encrypt document properties when saving as .xls file. The default value is true.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [ImageOrPrintOptions](../../aspose.cells/imagesaveoptions/imageorprintoptions/) { get; } | Additional image creation options. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indicates whether merge the areas of conditional formatting and validation before saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indicates whether refreshing chart cache data(Inherited from [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Gets the save file format.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indicates whether sorting external defined names before saving file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indicates whether sorting defined names before saving file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [StreamProvider](../../aspose.cells/imagesaveoptions/streamprovider/) { get; set; } | Gets or sets the IStreamProvider for exporting objects. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indicates whether updating smart art setting. The default value is false.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indicates whether validate merged cells before saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Gets or sets warning callback.(Inherited from [`SaveOptions`](../saveoptions/).) |

### Examples

```csharp
// Called: ImageSaveOptions saveOptions = new ImageSaveOptions(SaveFormat.Bmp);
public void Type_ImageSaveOptions()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET49614.xlsx");
            ImageSaveOptions saveOptions = new ImageSaveOptions(SaveFormat.Bmp);
           // saveOptions.StreamProvider = new StreamProvider();
            using (FileStream fs = File.Create(Constants.destPath + "CELLSNET49614_2.bmp"))
            {
                workbook.Save(fs, saveOptions);
            }
            Assert.AreEqual(FileFormatType.Bmp, FileFormatUtil.DetectFileFormat(Constants.destPath + "CELLSNET49614_2.bmp").FileFormatType);

        }
```

### See Also

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


