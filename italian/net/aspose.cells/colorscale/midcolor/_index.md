---
title: "ColorScale.MidColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ColorScale. Ottieni o imposta il colore gradiente per il valore medio nell'intervallo"
type: docs
url: /it/net/aspose.cells/colorscale/midcolor/
---
## ColorScale.MidColor property

Ottieni o imposta il colore gradiente per il valore intermedio nell'intervallo.

```csharp
public Color MidColor { get; set; }
```

### Esempi

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

### Vedi anche

* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


