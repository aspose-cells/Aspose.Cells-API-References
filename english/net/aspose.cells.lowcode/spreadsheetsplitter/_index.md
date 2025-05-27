---
title: Class SpreadsheetSplitter
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.LowCode.SpreadsheetSplitter class. Splits spreadsheet file into multiple parts
type: docs
url: /net/aspose.cells.lowcode/spreadsheetsplitter/
---
## SpreadsheetSplitter class

Splits spreadsheet file into multiple parts.

```csharp
public class SpreadsheetSplitter
```

## Methods

| Name | Description |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/spreadsheetsplitter/process/#process)(LowCodeSplitOptions) | Splits spreadsheet file into multiple parts. |
| static [Process](../../aspose.cells.lowcode/spreadsheetsplitter/process/#process_1)(string, string) | Splits given template file into multiple parts. |

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetSplitter
    {
        public static void Process(string templatePath, string outputPath)
        {
            Workbook templateWorkbook = new Workbook(templatePath);
            Workbook splitWorkbook = new Workbook();
            
            foreach (Worksheet sheet in templateWorkbook.Worksheets)
            {
                Worksheet newSheet = splitWorkbook.Worksheets.Add(sheet.Name);
                newSheet.Copy(sheet);
            }

            splitWorkbook.Save(outputPath);
        }
    }

    public class LowCodeClassSpreadsheetSplitterDemo
    {
        public static void Run()
        {
            SpreadsheetSplitter.Process("template.xlsx", "split.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


