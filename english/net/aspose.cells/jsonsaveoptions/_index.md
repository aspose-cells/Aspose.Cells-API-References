---
title: Class JsonSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.JsonSaveOptions class. Represents the options of saving the workbook as a JSON file
type: docs
url: /net/aspose.cells/jsonsaveoptions/
---
## JsonSaveOptions class

Represents the options of saving the workbook as a JSON file.

```csharp
public class JsonSaveOptions : SaveOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [JsonSaveOptions](jsonsaveoptions/)() | Creates options for saving json file. |

## Properties

| Name | Description |
| --- | --- |
| [AlwaysExportAsJsonObject](../../aspose.cells/jsonsaveoptions/alwaysexportasjsonobject/) { get; set; } | Indicates whether always exporting excel to json as object, even there is only a worksheet in the file. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | The folder for temporary files that may be used as data cache.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Make the workbook empty after saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | If true and the directory does not exist, the directory will be automatically created before saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indicates whether encrypt document properties when saving as .xls file. The default value is true.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [ExportArea](../../aspose.cells/jsonsaveoptions/exportarea/) { get; set; } | Gets or sets the exporting range. |
| [ExportAsString](../../aspose.cells/jsonsaveoptions/exportasstring/) { get; set; } | Exports the string value of the cells to json. |
| [ExportEmptyCells](../../aspose.cells/jsonsaveoptions/exportemptycells/) { get; set; } | Indicates whether exporting empty cells as null. |
| [ExportHyperlinkType](../../aspose.cells/jsonsaveoptions/exporthyperlinktype/) { get; set; } | Represents the type of exporting hyperlink to json. |
| [ExportNestedStructure](../../aspose.cells/jsonsaveoptions/exportnestedstructure/) { get; set; } | Exported as parent-child hierarchy Json structure. |
| [ExportStylePool](../../aspose.cells/jsonsaveoptions/exportstylepool/) { get; set; } | Indicates whether to export styles collectively or individually to each cell. |
| [HasHeaderRow](../../aspose.cells/jsonsaveoptions/hasheaderrow/) { get; set; } | Indicates whether the range contains header row. |
| [Indent](../../aspose.cells/jsonsaveoptions/indent/) { get; set; } | Indicates the indent. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indicates whether merge the areas of conditional formatting and validation before saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indicates whether refreshing chart cache data(Inherited from [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Gets the save file format.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [Schemas](../../aspose.cells/jsonsaveoptions/schemas/) { get; set; } | The original json schema of each worksheet. |
| [SheetIndexes](../../aspose.cells/jsonsaveoptions/sheetindexes/) { get; set; } | Represents the indexes of exported sheets. |
| [SkipEmptyRows](../../aspose.cells/jsonsaveoptions/skipemptyrows/) { get; set; } | Indicates whether skipping emtpy rows. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indicates whether sorting external defined names before saving file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indicates whether sorting defined names before saving file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [ToExcelStruct](../../aspose.cells/jsonsaveoptions/toexcelstruct/) { get; set; } | Indicates whether converting to json struct of the Excel file. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indicates whether updating smart art setting. The default value is false.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indicates whether validate merged cells before saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Gets or sets warning callback.(Inherited from [`SaveOptions`](../saveoptions/).) |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Json;
    using System;

    public class JsonSaveOptionsDemo
    {
        public static void JsonSaveOptionsExample()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fill some data into the worksheet
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            // Create an instance of JsonSaveOptions
            JsonSaveOptions saveOptions = new JsonSaveOptions
            {
                ExportHyperlinkType = JsonExportHyperlinkType.DisplayString,
                SkipEmptyRows = true,
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 },
                HasHeaderRow = true,
                ExportAsString = true,
                Indent = "  ",
                ExportNestedStructure = false,
                ExportEmptyCells = false,
                AlwaysExportAsJsonObject = false,
                ToExcelStruct = false,
                ClearData = false,
                CachedFileFolder = "C:\\Temp",
                ValidateMergedAreas = true,
                MergeAreas = false,
                SortNames = false,
                SortExternalNames = false,
                RefreshChartCache = false,
                UpdateSmartArt = false
            };

            // Save the workbook as a JSON file
            workbook.Save("JsonSaveOptionsExample.json", saveOptions);

            return;
        }
    }
}
```

### See Also

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


