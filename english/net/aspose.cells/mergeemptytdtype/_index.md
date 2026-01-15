---
title: Enum MergeEmptyTdType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.MergeEmptyTdType enum. Represents the merge type for an empty TD element when exporting a file to HTML
type: docs
url: /net/aspose.cells/mergeemptytdtype/
---
## MergeEmptyTdType enumeration

Represents the merge type for an empty TD element when exporting a file to HTML.

```csharp
public enum MergeEmptyTdType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Default | `0` | Display like MS Excel. |
| None | `1` | Empty TD elements will not be merged when exporting file to html. This will generate a significantly larger html file. |
| MergeForcely | `2` | Merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. If you want to import the html file to excel or export perfect grid lines when saving file to html, please keep the default value. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MergeEmptyTdTypeDemo
    {
        public static void MergeEmptyTdTypeExample()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells["A1"].PutValue("Data1");
            worksheet.Cells["B1"].PutValue("Data2");
            worksheet.Cells["C1"].PutValue("Data3");

            // Create HtmlSaveOptions and set the MergeEmptyTdType property
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.MergeEmptyTdType = MergeEmptyTdType.MergeForcely;

            // Save the workbook to HTML format
            workbook.Save("MergeEmptyTdTypeExample.html", saveOptions);

            Console.WriteLine("HTML file saved with MergeEmptyTdType.MergeForcely option.");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


