---
title: Class OoxmlSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.OoxmlSaveOptions class. Represents the options of saving office open xml file
type: docs
url: /net/aspose.cells/ooxmlsaveoptions/
---
## OoxmlSaveOptions class

Represents the options of saving office open xml file.

```csharp
public class OoxmlSaveOptions : SaveOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [OoxmlSaveOptions](ooxmlsaveoptions/#constructor)() | Creates the options for saving office open xml file. |
| [OoxmlSaveOptions](ooxmlsaveoptions/#constructor_1)(SaveFormat) | Creates the options for saving office open xml file. |

## Properties

| Name | Description |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | The cached file folder is used to store some large data.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Make the workbook empty after saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [CompressionType](../../aspose.cells/ooxmlsaveoptions/compressiontype/) { get; set; } | Gets and sets the compression type for ooxml file. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | If true and the directory does not exist, the directory will be automatically created before saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [EmbedOoxmlAsOleObject](../../aspose.cells/ooxmlsaveoptions/embedooxmlasoleobject/) { get; set; } | Indicates whether embedding Ooxml files of OleObject as ole object. |
| [EnableZip64](../../aspose.cells/ooxmlsaveoptions/enablezip64/) { get; set; } | Always use ZIP64 extensions when writing zip archives, even when unnecessary. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indicates whether encrypt document properties when saving as .xls file. The default value is true.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [ExportCellName](../../aspose.cells/ooxmlsaveoptions/exportcellname/) { get; set; } | Indicates if export cell name to Excel2007 .xlsx (.xlsm, .xltx, .xltm) file. If the output file may be accessed by SQL Server DTS, this value must be true. Setting the value to false will highly increase the performance and reduce the file size when creating large file. Default value is true. |
| [LightCellsDataProvider](../../aspose.cells/ooxmlsaveoptions/lightcellsdataprovider/) { get; set; } | The data provider for saving workbook in light mode. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indicates whether merge the areas of conditional formatting and validation before saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indicates whether refreshing chart cache data(Inherited from [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Gets the save file format.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indicates whether sorting external defined names before saving file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indicates whether sorting defined names before saving file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indicates whether updating smart art setting. The default value is false.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [UpdateZoom](../../aspose.cells/ooxmlsaveoptions/updatezoom/) { get; set; } | Indicates whether update scaling factor before saving the file if the PageSetup.FitToPagesWide and PageSetup.FitToPagesTall properties control how the worksheet is scaled. |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indicates whether validate merged cells before saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Gets or sets warning callback.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [WpsCompatibility](../../aspose.cells/ooxmlsaveoptions/wpscompatibility/) { get; set; } | Indicates whether to make the xls more compatible with WPS. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlSaveOptionsDemo
    {
        public static void OoxmlSaveOptionsExample()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fill some data into the worksheet
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Create an instance of OoxmlSaveOptions
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();

            // Setting properties
            saveOptions.ExportCellName = true;
            saveOptions.UpdateZoom = true;
            saveOptions.EnableZip64 = false;
            saveOptions.EmbedOoxmlAsOleObject = false;
            saveOptions.CompressionType = OoxmlCompressionType.Level6;
            saveOptions.ClearData = false;
            saveOptions.CachedFileFolder = "C:\\Temp";
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = false;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = false;
            saveOptions.RefreshChartCache = true;
            saveOptions.UpdateSmartArt = false;

            // Save the workbook with the specified options
            workbook.Save("OoxmlSaveOptionsExample.xlsx", saveOptions);

            return;
        }
    }
}
```

### See Also

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


