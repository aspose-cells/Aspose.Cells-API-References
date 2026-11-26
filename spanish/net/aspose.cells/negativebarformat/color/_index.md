---
title: "NegativeBarFormat.Color"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad NegativeBarFormat. Obtiene o establece un objeto FormatColor que puede usar para especificar el color de relleno de las barras de datos negativas"
type: docs
url: /es/net/aspose.cells/negativebarformat/color/
---
## NegativeBarFormat.Color property

Obtiene o establece un objeto FormatColor que puede usar para especificar el color de relleno de las barras de datos negativas.

```csharp
public Color Color { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class NegativeBarFormatPropertyColorDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["E3"].PutValue(-10);
            sheet.Cells["E4"].PutValue(20);
            sheet.Cells["F3"].PutValue(-30);
            sheet.Cells["F4"].PutValue(40);
            sheet.Cells["G3"].PutValue(-50);
            sheet.Cells["G4"].PutValue(60);

            // Crear formato condicional
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
            int idx = conds.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = conds[idx];

            // Configurar propiedades de barra de datos
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            cond.DataBar.ShowValue = false;

            // Configurar formato de barra negativa
            cond.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.Color = Color.White;
            cond.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Guarda el libro de trabajo
            workbook.Save("NegativeBarFormatColorDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("NegativeBarFormatPropertyColorDemo executed successfully.");
        }
    }
}
```

### Ver también

* class [NegativeBarFormat](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


