---
title: "Enumeración DataBarFillType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.DataBarFillType. Especifica cómo se rellena una barra de datos con color"
type: docs
url: /es/net/aspose.cells/databarfilltype/
---
## DataBarFillType enumeration

Especifica cómo se rellena una barra de datos con color.

```csharp
public enum DataBarFillType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Solid | `0` | La barra de datos se rellena con un color sólido. |
| Gradient | `1` | La barra de datos se rellena con un degradado de color. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarFillTypeDemo
    {
        public static void DataBarFillTypeExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();

            // Añadiendo una nueva hoja de cálculo al Libro
            Worksheet sheet = workbook.Worksheets[0];

            // Agrega un formato condicional vacío
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Establece el rango del formato condicional.
            CellArea ca = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);

            // Agregar condición
            int idx = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = fcs[idx];

            // Obtener Databar
            DataBar dataBar = cond.DataBar;

            // Establecer propiedades de Databar
            dataBar.Color = Color.Orange;
            dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MinCfvo.Value = 30;
            dataBar.ShowValue = false;
            dataBar.BarBorder.Type = DataBarBorderType.Solid;
            dataBar.BarBorder.Color = Color.Plum;
            dataBar.BarFillType = DataBarFillType.Solid;
            dataBar.AxisColor = Color.Red;
            dataBar.AxisPosition = DataBarAxisPosition.Midpoint;
            dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.Color = Color.White;
            dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Asignar valores de celda
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            // Guardando el archivo Excel
            workbook.Save("DataBarFillTypeExample.xlsx");
            workbook.Save("DataBarFillTypeExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


