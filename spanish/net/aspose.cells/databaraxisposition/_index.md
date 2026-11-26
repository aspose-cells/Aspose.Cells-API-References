---
title: "Enum DataBarAxisPosition"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.DataBarAxisPosition. Especifica la posición del eje para un rango de celdas con formato condicional como barras de datos"
type: docs
url: /es/net/aspose.cells/databaraxisposition/
---
## DataBarAxisPosition enumeration

Especifica la posición del eje para un rango de celdas con formato condicional como barras de datos.

```csharp
public enum DataBarAxisPosition
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Automatic | `0` | Muestra el eje en una posición variable basada en la proporción del valor negativo mínimo al valor positivo máximo en el rango. Los valores positivos se muestran de izquierda a derecha. Los valores negativos se muestran de derecha a izquierda. Cuando todos los valores son positivos o todos son negativos, no se muestra ningún eje. |
| Midpoint | `1` | Muestra el eje en el punto medio de la celda sin importar el conjunto de valores en el rango. Los valores positivos se muestran de izquierda a derecha. Los valores negativos se muestran de derecha a izquierda. |
| None | `2` | No se muestra eje, y tanto los valores positivos como los negativos se muestran de izquierda a derecha. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarAxisPositionDemo
    {
        public static void DataBarAxisPositionExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();
            
            // Accediendo a la primera hoja de cálculo en el libro de trabajo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Añadiendo una regla de formato condicional
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Estableciendo el rango de formato condicional
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);
            
            // Añadiendo una condición de barra de datos
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];
            DataBar dataBar = fc.DataBar;
            
            // Estableciendo propiedades para la barra de datos
            dataBar.Color = Color.Orange;
            dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MinCfvo.Value = 30;
            dataBar.ShowValue = false;
            dataBar.BarBorder.Type = DataBarBorderType.Solid;
            dataBar.BarBorder.Color = Color.Plum;
            dataBar.BarFillType = DataBarFillType.Solid;
            dataBar.AxisColor = Color.Red;
            dataBar.AxisPosition = DataBarAxisPosition.Midpoint; // Using DataBarAxisPosition enum
            dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.Color = Color.White;
            dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.BorderColor = Color.Yellow;
            
            // Asignando valores a las celdas
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(120);
            worksheet.Cells["A3"].PutValue(260);
            
            // Guardando el archivo Excel
            workbook.Save("DataBarAxisPositionExample.xlsx");
            workbook.Save("DataBarAxisPositionExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


