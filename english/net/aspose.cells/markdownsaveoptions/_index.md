---
title: Class MarkdownSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.MarkdownSaveOptions class. Represents the save options for markdown
type: docs
url: /net/aspose.cells/markdownsaveoptions/
---
## MarkdownSaveOptions class

Represents the save options for markdown.

```csharp
public class MarkdownSaveOptions : SaveOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [MarkdownSaveOptions](markdownsaveoptions/)() | Creates options for saving markdown document |

## Properties

| Name | Description |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | The cached file folder is used to store some large data.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Make the workbook empty after saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | If true and the directory does not exist, the directory will be automatically created before saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [Encoding](../../aspose.cells/markdownsaveoptions/encoding/) { get; set; } | Gets and sets the default encoding. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indicates whether encrypt document properties when saving as .xls file. The default value is true.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [FormatStrategy](../../aspose.cells/markdownsaveoptions/formatstrategy/) { get; set; } | Gets and sets the format strategy when exporting the cell value as string. |
| [LightCellsDataProvider](../../aspose.cells/markdownsaveoptions/lightcellsdataprovider/) { get; set; } | The Data provider to provide cells data for saving workbook in light mode. |
| [LineSeparator](../../aspose.cells/markdownsaveoptions/lineseparator/) { get; set; } | Gets and sets the line separator. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indicates whether merge the areas of conditional formatting and validation before saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indicates whether refreshing chart cache data(Inherited from [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Gets the save file format.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indicates whether sorting external defined names before saving file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indicates whether sorting defined names before saving file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indicates whether updating smart art setting. The default value is false.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indicates whether validate merged cells before saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Gets or sets warning callback.(Inherited from [`SaveOptions`](../saveoptions/).) |

### Examples

```csharp
[C#]

namespace Demos
{
    using Aspose.Cells;
    using System;
    using System.Text;

    public class MarkdownSaveOptionsDemo
    {
        public static void MarkdownSaveOptionsExample()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Create an instance of MarkdownSaveOptions
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
            {
                Encoding = Encoding.UTF8,
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                LineSeparator = "\n",
                ClearData = false,
                CachedFileFolder = "C:\\Temp",
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = false,
                SortExternalNames = false,
                RefreshChartCache = false,
                UpdateSmartArt = false
            };

            // Save the workbook as a Markdown file
            workbook.Save("MarkdownSaveOptionsExample.md", saveOptions);

            Console.WriteLine("Workbook saved as Markdown file successfully.");
        }
    }
}
```

### See Also

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


