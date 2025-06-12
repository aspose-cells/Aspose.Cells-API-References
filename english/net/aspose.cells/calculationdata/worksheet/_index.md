---
title: CalculationData.Worksheet
second_title: Aspose.Cells for .NET API Reference
description: CalculationData property. Gets the Worksheet object where the function is in
type: docs
url: /net/aspose.cells/calculationdata/worksheet/
---
## CalculationData.Worksheet property

Gets the Worksheet object where the function is in.

```csharp
public Worksheet Worksheet { get; }
```

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationDataPropertyWorksheetDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Set sample data in cells
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(25);

            // Calculate array formula using Worksheet property
            object result = worksheet.CalculateArrayFormula(
                "=IFERROR(A2:A4,B2:B4)", new CalculationOptions());

            // Output the result (assuming it's an array)
            if (result is object[,] arrayResult)
            {
                Console.WriteLine("Calculation Results:");
                for (int i = 0; i < arrayResult.GetLength(0); i++)
                {
                    Console.WriteLine(arrayResult[i, 0]);
                }
            }
        }
    }
}
```

### See Also

* class [Worksheet](../../worksheet/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


