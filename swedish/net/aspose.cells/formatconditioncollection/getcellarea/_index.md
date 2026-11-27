---
title: "FormatConditionCollection.GetCellArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormatConditionCollection-metoden. Hämtar det villkorligt formaterade cellområdet efter index"
type: docs
url: /sv/net/aspose.cells/formatconditioncollection/getcellarea/
---
## FormatConditionCollection.GetCellArea method

Hämtar det villkorligt formaterade cellområdet efter index.

```csharp
public CellArea GetCellArea(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | indexet för det villkorligt formaterade cellområdet. |

### Returvärde

det villkorligt formaterade cellområdet

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodGetCellAreaWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].Value = i + j;
                }
            }

            // Lägg till villkorsstyrd formatering
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Ange området för villkorsformatering
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 7;
            area.EndColumn = 3;
            fcc.AddArea(area);

            // Lägg till villkor och ange stil
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "10");
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            fcc[conditionIndex].Style = style;

            // Hämta och visa information om cellområdet
            CellArea retrievedArea = fcc.GetCellArea(0);
            Console.WriteLine("Conditional Format Area:");
            Console.WriteLine($"StartRow: {retrievedArea.StartRow}");
            Console.WriteLine($"StartColumn: {retrievedArea.StartColumn}");
            Console.WriteLine($"EndRow: {retrievedArea.EndRow}");
            Console.WriteLine($"EndColumn: {retrievedArea.EndColumn}");

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


