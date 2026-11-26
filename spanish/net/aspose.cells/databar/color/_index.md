---
title: "DataBar.Color"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataBar. Obtener o establecer el Color de esta DataBar"
type: docs
url: /es/net/aspose.cells/databar/color/
---
## DataBar.Color property

Obtener o establecer el Color de esta DataBar.

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
    public class DataBarPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un rango de celdas
            CellArea area = new CellArea();
            area.StartRow = 2;
            area.StartColumn = 4;
            area.EndRow = 3;
            area.EndColumn = 6;

            // Agregar algunos datos de ejemplo
            worksheet.Cells["E3"].PutValue(10);
            worksheet.Cells["F3"].PutValue(20);
            worksheet.Cells["G3"].PutValue(30);
            worksheet.Cells["E4"].PutValue(15);
            worksheet.Cells["F4"].PutValue(25);
            worksheet.Cells["G4"].PutValue(35);

            // Agregar formato condicional con barra de datos
            int formatIndex = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection conditions = worksheet.ConditionalFormattings[formatIndex];
            int index = conditions.AddCondition(FormatConditionType.DataBar);
            FormatCondition condition = conditions[index];

            // Establecer propiedades de la barra de datos, incluido el Color
            condition.DataBar.Color = Color.Orange;
            condition.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            condition.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            condition.DataBar.ShowValue = false;

            // Establecer propiedades del borde
            condition.DataBar.BarBorder.Type = DataBarBorderType.Solid;
            condition.DataBar.BarBorder.Color = Color.Plum;

            // Establecer tipo de relleno
            condition.DataBar.BarFillType = DataBarFillType.Gradient;

            // Establecer propiedades del eje
            condition.DataBar.AxisColor = Color.Red;
            condition.DataBar.AxisPosition = DataBarAxisPosition.Automatic;

            // Establecer propiedades de la barra negativa
            condition.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            condition.DataBar.NegativeBarFormat.Color = Color.White;
            condition.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            condition.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Aplicar el formato al rango
            conditions.AddArea(area);

            // Guarda el libro de trabajo
            workbook.Save("DataBarPropertyColorDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("DataBarPropertyColorDemo executed successfully.");
        }
    }
}
```

### Ver también

* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


