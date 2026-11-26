---
title: "DataBar.NegativeBarFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataBar. Obtiene el objeto NegativeBarFormat asociado a una regla de formato condicional de barra de datos"
type: docs
url: /es/net/aspose.cells/databar/negativebarformat/
---
## DataBar.NegativeBarFormat property

Obtiene el objeto NegativeBarFormat asociado a una regla de formato condicional de barra de datos.

```csharp
public NegativeBarFormat NegativeBarFormat { get; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyNegativeBarFormatDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de muestra con valores negativos
            sheet.Cells["E3"].PutValue(-10);
            sheet.Cells["E4"].PutValue(20);
            sheet.Cells["F3"].PutValue(-30);
            sheet.Cells["F4"].PutValue(40);
            sheet.Cells["G3"].PutValue(-50);
            sheet.Cells["G4"].PutValue(60);

            // Agregar formato condicional de barra de datos
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conditions = sheet.ConditionalFormattings[formatIndex];
            int index = conditions.AddCondition(FormatConditionType.DataBar);
            FormatCondition condition = conditions[index];

            // Establecer propiedades de la barra de datos
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

            // Configurar formato de barra negativa
            condition.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            condition.DataBar.NegativeBarFormat.Color = Color.White;
            condition.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            condition.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Guarda el libro de trabajo
            workbook.Save("DataBarNegativeFormatDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [NegativeBarFormat](../../negativebarformat/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


