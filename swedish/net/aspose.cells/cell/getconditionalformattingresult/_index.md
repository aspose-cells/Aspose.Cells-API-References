---
title: "Cell.GetConditionalFormattingResult"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-metod. Hämta resultatet av den villkorliga formateringen"
type: docs
url: /sv/net/aspose.cells/cell/getconditionalformattingresult/
---
## Cell.GetConditionalFormattingResult method

Hämta resultatet av den villkorsstyrda formateringen.

```csharp
public ConditionalFormattingResult GetConditionalFormattingResult()
```

### Anmärkningar

Returnerar null om ingen villkorlig formatering har tillämpats på den här cellen,

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetConditionalFormattingResultDemo
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

            // Lägg till villkorsstyrd formatering
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            fcc.AddArea(area);
            
            // Ange villkor och stil
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "15", "35");
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            fcc[conditionIndex].Style = style;

            // Hämta resultatet av villkorlig formatering för en cell
            Cell cell = worksheet.Cells["A2"];
            ConditionalFormattingResult result = cell.GetConditionalFormattingResult();
            
            // Utskriftsresultat
            Console.WriteLine("Cell A2 meets condition: " + (result.ConditionalStyle != null));
            Console.WriteLine("Applied font color: " + result.ConditionalStyle.Font.Color);
        }
    }
}
```

### Se även

* class [ConditionalFormattingResult](../../conditionalformattingresult/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


