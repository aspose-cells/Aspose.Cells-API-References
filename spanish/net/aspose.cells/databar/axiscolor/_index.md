---
title: "DataBar.AxisColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataBar. Obtiene el color del eje para celdas con formato condicional como barras de datos"
type: docs
url: /es/net/aspose.cells/databar/axiscolor/
---
## DataBar.AxisColor property

Obtiene el color del eje para las celdas con formato condicional como barras de datos.

```csharp
public Color AxisColor { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyAxisColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Establecer datos de muestra
            sheet.Cells["E3"].PutValue(10);
            sheet.Cells["E4"].PutValue(20);
            sheet.Cells["F3"].PutValue(30);
            sheet.Cells["F4"].PutValue(40);
            sheet.Cells["G3"].PutValue(-15);
            sheet.Cells["G4"].PutValue(-25);

            // Agregar formato condicional de barra de datos
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
            int idx = conds.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = conds[idx];

            // Establecer propiedades de la barra de datos
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            cond.DataBar.ShowValue = false;
            cond.DataBar.BarBorder.Type = DataBarBorderType.Solid;
            cond.DataBar.BarBorder.Color = Color.Plum;
            cond.DataBar.BarFillType = DataBarFillType.Solid;
            
            // Demostrar la propiedad AxisColor
            cond.DataBar.AxisColor = Color.Red;
            cond.DataBar.AxisPosition = DataBarAxisPosition.Midpoint;

            // Establecer formato de barra negativa
            cond.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.Color = Color.White;
            cond.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Guarda el libro de trabajo
            workbook.Save("DataBarAxisColorDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


