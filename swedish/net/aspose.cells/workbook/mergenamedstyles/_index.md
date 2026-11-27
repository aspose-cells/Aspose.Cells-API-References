---
title: "Workbook.MergeNamedStyles"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Slår samman namngivna stilar från den andra Excel-filen"
type: docs
url: /sv/net/aspose.cells/workbook/mergenamedstyles/
---
## Workbook.MergeNamedStyles method

Slår samman namngivna format från den andra Excel-filen.

```csharp
public void MergeNamedStyles(Workbook source)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| källa | Arbetsbok | Den andra filen |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodMergeNamedStylesWithWorkbookDemo
    {
        public static void Run()
        {
            // Skapa målarbetsboken (den som kommer att ta emot namngivna stilar)
            using (Workbook targetWorkbook = new Workbook())
            {
                // Lägg till lite data i målarbetsboken för kontext
                Worksheet targetSheet = targetWorkbook.Worksheets[0];
                targetSheet.Cells["A1"].PutValue("Target Workbook");

                // Skapa källarbetsboken (den som innehåller namngivna stilar att slå samman)
                using (Workbook sourceWorkbook = new Workbook())
                {
                    // Lägg till lite data i källarbetsboken för kontext
                    Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
                    sourceSheet.Cells["A1"].PutValue("Source Workbook");

                    try
                    {
                        // Slå samman namngivna stilar från sourceWorkbook till targetWorkbook
                        targetWorkbook.MergeNamedStyles(sourceWorkbook);

                        Console.WriteLine("MergeNamedStyles executed successfully.");

                        // Spara den resulterande arbetsboken
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

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


