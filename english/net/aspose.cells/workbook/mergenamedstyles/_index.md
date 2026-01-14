---
title: Workbook.MergeNamedStyles
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Merges named styles from the other Excel file
type: docs
url: /net/aspose.cells/workbook/mergenamedstyles/
---
## Workbook.MergeNamedStyles method

Merges named styles from the other Excel file.

```csharp
public void MergeNamedStyles(Workbook source)
```

| Parameter | Type | Description |
| --- | --- | --- |
| source | Workbook | The other file |

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodMergeNamedStylesWithWorkbookDemo
    {
        public static void Run()
        {
            // Create the target workbook (the one that will receive named styles)
            using (Workbook targetWorkbook = new Workbook())
            {
                // Add some data to the target workbook for context
                Worksheet targetSheet = targetWorkbook.Worksheets[0];
                targetSheet.Cells["A1"].PutValue("Target Workbook");

                // Create the source workbook (the one that contains named styles to merge)
                using (Workbook sourceWorkbook = new Workbook())
                {
                    // Add some data to the source workbook for context
                    Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
                    sourceSheet.Cells["A1"].PutValue("Source Workbook");

                    try
                    {
                        // Merge named styles from sourceWorkbook into targetWorkbook
                        targetWorkbook.MergeNamedStyles(sourceWorkbook);

                        Console.WriteLine("MergeNamedStyles executed successfully.");

                        // Save the resulting workbook
                        string outputPath = "MergedNamedStylesDemo.xlsx";
                        targetWorkbook.Save(outputPath, SaveFormat.Xlsx);
                        Console.WriteLine($"Workbook saved to '{outputPath}'.");
                    }
                    catch (Exception ex)
                    {
                        Console.WriteLine($"Error during MergeNamedStyles: {ex.Message}");
                    }
                }
            }
        }
    }
}
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


