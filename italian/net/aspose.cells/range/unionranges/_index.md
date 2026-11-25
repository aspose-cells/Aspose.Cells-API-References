---
title: "Range.UnionRanges"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Restituisce il risultato dell'unione di due intervalli"
type: docs
url: /it/net/aspose.cells/range/unionranges/
---
## Range.UnionRanges method

Restituisce il risultato dell'unione di due intervalli.

```csharp
public UnionRange UnionRanges(Range[] ranges)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| intervalli | Range[] | L'intervallo |

### Valore di ritorno

L'unione di due intervalli.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodUnionRangesWithRangeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio nelle celle
            worksheet.Cells["A1"].PutValue("Range 1");
            worksheet.Cells["B1"].PutValue("Data 1");
            worksheet.Cells["C1"].PutValue("Data 2");
            worksheet.Cells["A5"].PutValue("Range 2");
            worksheet.Cells["B5"].PutValue("Data 3");
            worksheet.Cells["C5"].PutValue("Data 4");

            // Crea intervalli da unire
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:C3");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A5:C7");

            try
            {
                // Chiama UnionRanges con parametro Range[]
                Aspose.Cells.Range[] rangesToUnion = new Aspose.Cells.Range[] { range1, range2 };
                UnionRange unionRange = range1.UnionRanges(rangesToUnion);

                // Applica lo stile per mostrare l'intervallo unito
                Style style = workbook.CreateStyle();
                style.BackgroundColor = System.Drawing.Color.LightBlue;
                unionRange.ApplyStyle(style, new StyleFlag { All = true });

                Console.WriteLine($"Union range created successfully. Address: {unionRange.RefersTo}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnionRanges method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("UnionRangesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [UnionRange](../../unionrange/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


