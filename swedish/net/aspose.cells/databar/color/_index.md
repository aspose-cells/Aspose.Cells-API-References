---
title: "DataBar.Color"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataBar property. Hämta eller ange färgen på denna DataBar"
type: docs
url: /sv/net/aspose.cells/databar/color/
---
## DataBar.Color property

Hämta eller ange färgen för denna DataBar.

```csharp
public Color Color { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa ett cellområde
            CellArea area = new CellArea();
            area.StartRow = 2;
            area.StartColumn = 4;
            area.EndRow = 3;
            area.EndColumn = 6;

            // Lägg till lite exempeldata
            worksheet.Cells["E3"].PutValue(10);
            worksheet.Cells["F3"].PutValue(20);
            worksheet.Cells["G3"].PutValue(30);
            worksheet.Cells["E4"].PutValue(15);
            worksheet.Cells["F4"].PutValue(25);
            worksheet.Cells["G4"].PutValue(35);

            // Lägg till villkorlig formatering med datastapel
            int formatIndex = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection conditions = worksheet.ConditionalFormattings[formatIndex];
            int index = conditions.AddCondition(FormatConditionType.DataBar);
            FormatCondition condition = conditions[index];

            // Ställ in datastapelns egenskaper inklusive färg
            condition.DataBar.Color = Color.Orange;
            condition.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            condition.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            condition.DataBar.ShowValue = false;

            // Ställ in kantegenskaper
            condition.DataBar.BarBorder.Type = DataBarBorderType.Solid;
            condition.DataBar.BarBorder.Color = Color.Plum;

            // Ställ in fyllningstyp
            condition.DataBar.BarFillType = DataBarFillType.Gradient;

            // Ställ in axelns egenskaper
            condition.DataBar.AxisColor = Color.Red;
            condition.DataBar.AxisPosition = DataBarAxisPosition.Automatic;

            // Ställ in negativa stapelns egenskaper
            condition.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            condition.DataBar.NegativeBarFormat.Color = Color.White;
            condition.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            condition.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Tillämpa formateringen på området
            conditions.AddArea(area);

            // Spara arbetsboken
            workbook.Save("DataBarPropertyColorDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("DataBarPropertyColorDemo executed successfully.");
        }
    }
}
```

### Se även

* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


