---
title: "ConditionalFormattingResult.ColorScaleResult"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ConditionalFormattingResult. Obtiene el color de visualización de la escala de colores"
type: docs
url: /es/net/aspose.cells/conditionalformattingresult/colorscaleresult/
---
## ConditionalFormattingResult.ColorScaleResult property

Obtiene el color de visualización de la escala de colores.

```csharp
public Color ColorScaleResult { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingResultPropertyColorScaleResultDemo
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
            
            Color colorScaleResult = cfr.ColorScaleResult;
            Console.WriteLine("Color Scale Result for cell B2: " + colorScaleResult);

            workbook.Save("ColorScaleResultDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ConditionalFormattingResult](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


