---
title: "Worksheet.ConditionalFormattings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Hämtar ConditionalFormattings i arbetsbladet"
type: docs
url: /sv/net/aspose.cells/worksheet/conditionalformattings/
---
## Worksheet.ConditionalFormattings property

Hämtar ConditionalFormattings i kalkylbladet.

```csharp
public ConditionalFormattingCollection ConditionalFormattings { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyConditionalFormattingsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);

            // Skapa villkorlig formatering
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            
            // Ange intervallet
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Lägg till villkor
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "15", null);
            FormatCondition fc = fcc[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Red;

            // Spara arbetsboken
            workbook.Save("ConditionalFormattingDemo.xlsx");
        }
    }
}
```

### Se även

* class [ConditionalFormattingCollection](../../conditionalformattingcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


