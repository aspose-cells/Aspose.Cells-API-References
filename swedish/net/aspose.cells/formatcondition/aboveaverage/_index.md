---
title: "FormatCondition.AboveAverage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormatCondition-egenskap. Hämta den villkorliga formateringens AboveAverage-instans. Standardinstansens regel markerar celler som ligger över genomsnittet för alla värden i området. Giltig endast för typen AboveAverage"
type: docs
url: /sv/net/aspose.cells/formatcondition/aboveaverage/
---
## FormatCondition.AboveAverage property

Hämta den villkorliga formateringens "AboveAverage"-instans. Standardinstansens regel markerar celler som ligger över genomsnittet för alla värden i intervallet. Giltig endast för typ = AboveAverage.

```csharp
public AboveAverage AboveAverage { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyAboveAverageDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Lägg till villkorlig formatering för över genomsnittet
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.AboveAverage);
            fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 4, EndColumn = 0 });

            // Ställ in för att markera värden över genomsnittet
            FormatCondition fc = fcc[0];
            fc.AboveAverage.IsAboveAverage = true;
            fc.Style.BackgroundColor = Color.Yellow;

            // Lägg till villkorlig formatering för under genomsnittet
            index = worksheet.ConditionalFormattings.Add();
            fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.AboveAverage);
            fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 1, EndRow = 4, EndColumn = 1 });

            // Ställ in för att markera värden under genomsnittet
            fc = fcc[0];
            fc.AboveAverage.IsAboveAverage = false;
            fc.Style.BackgroundColor = Color.LightBlue;

            // Spara arbetsboken
            workbook.Save("AboveAverageConditionDemo.xlsx");
        }
    }
}
```

### Se även

* class [AboveAverage](../../aboveaverage/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


