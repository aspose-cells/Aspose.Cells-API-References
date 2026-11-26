---
title: "Class DataBar"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.DataBar. Describe la regla de formato condicional DataBar. Esta regla de formato condicional muestra una barra de datos graduada en el rango de celdas"
type: docs
url: /es/net/aspose.cells/databar/
---
## DataBar class

Describe la regla de formato condicional DataBar. Esta regla de formato condicional muestra una barra de datos graduada en el rango de celdas.

```csharp
public class DataBar
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AxisColor](../../aspose.cells/databar/axiscolor/) { get; set; } | Obtiene el color del eje para las celdas con formato condicional como barras de datos. |
| [AxisPosition](../../aspose.cells/databar/axisposition/) { get; set; } | Obtiene o establece la posición del eje de las barras de datos especificado por una regla de formato condicional. |
| [BarBorder](../../aspose.cells/databar/barborder/) { get; } | Obtiene un objeto que especifica el borde de una barra de datos. |
| [BarFillType](../../aspose.cells/databar/barfilltype/) { get; set; } | Obtiene o establece cómo se rellena una barra de datos con color. |
| [Color](../../aspose.cells/databar/color/) { get; set; } | Obtener o establecer el Color de esta DataBar. |
| [Direction](../../aspose.cells/databar/direction/) { get; set; } | Obtiene o establece la dirección en que se muestra el databar. |
| [MaxCfvo](../../aspose.cells/databar/maxcfvo/) { get; } | Obtener o establecer el objeto de valor máximo de esta DataBar. No se puede establecer null o CFValueObject con tipo FormatConditionValueType.Min en él. |
| [MaxLength](../../aspose.cells/databar/maxlength/) { get; set; } | Representa la longitud máxima de la barra de datos. |
| [MinCfvo](../../aspose.cells/databar/mincfvo/) { get; } | Obtener o establecer el objeto de valor mínimo de esta DataBar. No se puede establecer null o CFValueObject con tipo FormatConditionValueType.Max en él. |
| [MinLength](../../aspose.cells/databar/minlength/) { get; set; } | Representa la longitud mínima de la barra de datos. |
| [NegativeBarFormat](../../aspose.cells/databar/negativebarformat/) { get; } | Obtiene el objeto NegativeBarFormat asociado a una regla de formato condicional de barra de datos. |
| [ShowValue](../../aspose.cells/databar/showvalue/) { get; set; } | Obtener o establecer la bandera que indica si se deben mostrar los valores de las celdas a las que se aplica esta barra de datos. El valor predeterminado es true. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [ToImage](../../aspose.cells/databar/toimage/)(Cell, ImageOrPrintOptions) | Renderizar la barra de datos en la celda a una matriz de bytes de imagen. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarDemo
    {
        public static void DataBarExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agrega un formato condicional vacío
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Establece el rango de formato condicional
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            // Agregar condición
            int idx = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = fcs[idx];

            // Obtener DataBar
            DataBar dataBar = cond.DataBar;

            // Establecer propiedades de DataBar
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
            Aspose.Cells.Cell cell1 = sheet.Cells["A1"];
            cell1.PutValue(10);
            Aspose.Cells.Cell cell2 = sheet.Cells["A2"];
            cell2.PutValue(120);
            Aspose.Cells.Cell cell3 = sheet.Cells["A3"];
            cell3.PutValue(260);

            // Guardando el archivo Excel
            workbook.Save("DataBarExample.xlsx");
            workbook.Save("DataBarExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


