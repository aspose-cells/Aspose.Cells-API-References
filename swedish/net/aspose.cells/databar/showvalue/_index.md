---
title: "DataBar.ShowValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataBar property. Hämta eller ange flaggan som indikerar om värdena i cellerna som denna datastapel tillämpas på ska visas. Standardvärdet är true"
type: docs
url: /sv/net/aspose.cells/databar/showvalue/
---
## DataBar.ShowValue property

Hämta eller ange flaggan som indikerar om värdena i cellerna som denna data bar tillämpas på ska visas. Standardvärdet är true.

```csharp
public bool ShowValue { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarPropertyShowValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);

            // Lägg till villkorlig formatering för datastaplar
            int idx = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[idx];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 3;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Lägg till villkor för datastapel
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcc[conditionIndex];
            
            // Ställ in egenskaper för datastaplar
            fc.DataBar.MinCfvo.Type = FormatConditionValueType.Min;
            fc.DataBar.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.DataBar.Color = Color.Green;
            
            // Demonstrera ShowValue-egenskapen
            fc.DataBar.ShowValue = true; // Show cell values along with data bars
            
            // Spara arbetsboken
            workbook.Save("DataBarShowValueDemo.xlsx");
            
            Console.WriteLine("DataBar ShowValue demo completed. Output file: DataBarShowValueDemo.xlsx");
        }
    }
}
```

### Se även

* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


