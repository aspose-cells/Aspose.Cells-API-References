---
title: "NegativeBarFormat.BorderColorType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad NegativeBarFormat. Indica si se debe usar el mismo color de borde que las barras de datos positivas"
type: docs
url: /es/net/aspose.cells/negativebarformat/bordercolortype/
---
## NegativeBarFormat.BorderColorType property

Indica si se debe usar el mismo color de borde que las barras de datos positivas.

```csharp
public DataBarNegativeColorType BorderColorType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class NegativeBarFormatPropertyBorderColorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["E3"].PutValue(-10);
            sheet.Cells["E4"].PutValue(20);
            sheet.Cells["F3"].PutValue(-30);
            sheet.Cells["F4"].PutValue(40);
            sheet.Cells["G3"].PutValue(-50);
            sheet.Cells["G4"].PutValue(60);

            // Agregar formato condicional de barra de datos
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
            int idx = conds.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = conds[idx];

            // Configurar barra de datos
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            cond.DataBar.ShowValue = false;

            // Establecer el borde de la barra de datos
            cond.DataBar.BarBorder.Type = DataBarBorderType.Solid;
            cond.DataBar.BarBorder.Color = Color.Plum;

            // Establecer formato de barra negativa
            cond.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.Color = Color.White;
            
            // Demostrar la propiedad BorderColorType
            cond.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Guarda el libro de trabajo
            workbook.Save("NegativeBarFormatBorderColorTypeDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Demo completed. File saved.");
        }
    }
}
```

### Ver también

* enum [DataBarNegativeColorType](../../databarnegativecolortype/)
* class [NegativeBarFormat](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


