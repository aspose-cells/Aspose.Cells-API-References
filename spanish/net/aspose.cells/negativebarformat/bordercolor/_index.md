---
title: "NegativeBarFormat.BorderColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad NegativeBarFormat. Obtiene o establece un objeto FormatColor que puede usar para especificar el color del borde de las barras de datos negativas"
type: docs
url: /es/net/aspose.cells/negativebarformat/bordercolor/
---
## NegativeBarFormat.BorderColor property

Obtiene o establece un objeto FormatColor que puede usar para especificar el color del borde de las barras de datos negativas.

```csharp
public Color BorderColor { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NegativeBarFormatPropertyBorderColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            CellArea ca = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);

            int idx = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = fcs[idx];
            DataBar dataBar = cond.DataBar;

            dataBar.Color = Color.Orange;
            dataBar.BarBorder.Type = DataBarBorderType.Solid;
            dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            sheet.Cells["A1"].PutValue(-10);
            sheet.Cells["A2"].PutValue(50);
            sheet.Cells["A3"].PutValue(-100);

            workbook.Save("NegativeBarFormatBorderColorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [NegativeBarFormat](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


