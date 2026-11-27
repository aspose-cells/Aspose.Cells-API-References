---
title: "CalculationData.CellRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CalculationData-egenskap. Hämtar radindex för cellen där funktionen finns"
type: docs
url: /sv/net/aspose.cells/calculationdata/cellrow/
---
## CalculationData.CellRow property

Hämtar radindexet för cellen där funktionen är.

```csharp
public int CellRow { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationDataPropertyCellRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange några exempeldata
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");

            // Ställ in beräkningsalternativ
            CalculationOptions opts = new CalculationOptions();
            opts.CustomEngine = new CustomCalculationEngine();

            // Beräkna formler
            workbook.CalculateFormula(opts);

            // Åtkomst till den beräknade cellen och demonstrera CellRow-egenskapen
            Cell calculatedCell = worksheet.Cells["A3"];
            Console.WriteLine("Calculated cell is at row: " + calculatedCell.Row);
        }
    }

    public class CustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            // Demonstrera åtkomst till radinformation från beräkningsdata
            if (data != null)
            {
                Console.WriteLine("Current calculation is for row: " + data.CellRow);
            }
        }
    }
}
```

### Se även

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


