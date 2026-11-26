---
title: "ColorScale.MidColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ColorScale. Получить или установить градиентный цвет для среднего значения в диапазоне"
type: docs
url: /ru/net/aspose.cells/colorscale/midcolor/
---
## ColorScale.MidColor property

Получить или установить градиентный цвет для среднего значения в диапазоне.

```csharp
public Color MidColor { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ColorScalePropertyMidColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            CellArea ca = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];

            fc.ColorScale.Is3ColorScale = true;
            fc.ColorScale.MinColor = Color.Red;
            fc.ColorScale.MidColor = Color.Yellow;
            fc.ColorScale.MaxColor = Color.Green;

            for (int i = 0; i <= 5; i++)
            {
                for (int j = 0; j <= 5; j++)
                {
                    worksheet.Cells[i, j].PutValue(i * j);
                }
            }

            Cell cell = worksheet.Cells["B2"];
            ConditionalFormattingResult cfr = cell.GetConditionalFormattingResult();
            Console.WriteLine("MidColor used in scale: " + fc.ColorScale.MidColor);
            Console.WriteLine("Actual color for cell B2: " + cfr.ColorScaleResult);

            workbook.Save("ColorScaleMidColorDemo.xlsx");
        }
    }
}
```

### См. также

* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


