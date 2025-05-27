---
title: Class SpreadsheetMerger
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.LowCode.SpreadsheetMerger class. Merges multiple template files into one
type: docs
url: /net/aspose.cells.lowcode/spreadsheetmerger/
---
## SpreadsheetMerger class

Merges multiple template files into one.

```csharp
public class SpreadsheetMerger
```

## Methods

| Name | Description |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/spreadsheetmerger/process/#process)(LowCodeMergeOptions) | Merges multiple template files into one. |
| static [Process](../../aspose.cells.lowcode/spreadsheetmerger/process/#process_1)(string[], string) | Merge given template files. |

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetMerger
    {
        public static void Process(string[] inputFiles, string outputFile)
        {
            Workbook outputWorkbook = new Workbook();
            outputWorkbook.Worksheets.Clear();

            foreach (string file in inputFiles)
            {
                Workbook sourceWorkbook = new Workbook(file);
                foreach (Worksheet sourceSheet in sourceWorkbook.Worksheets)
                {
                    Worksheet outputSheet = outputWorkbook.Worksheets.Add(sourceSheet.Name);
                    outputSheet.Copy(sourceSheet);
                }
            }

            outputWorkbook.Save(outputFile);
        }
    }

    public class LowCodeClassSpreadsheetMergerDemo
    {
        public static void Run()
        {
            SpreadsheetMerger.Process(new string[] { "template2.xlsx", "template2.xlsx" }, "res.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


