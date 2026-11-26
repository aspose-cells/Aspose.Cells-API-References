---
title: "Enum FormattingType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.FormattingType enum. Representa el tipo de formato aplicado a un objeto Area o a un objeto Line"
type: docs
url: /es/net/aspose.cells.charts/formattingtype/
---
## FormattingType enumeration

Representa el tipo de formato aplicado a un objeto [`Area`](../../aspose.cells.drawing/area/) o a un objeto [`Line`](../../aspose.cells.drawing/line/).

```csharp
public enum FormattingType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Automatic | `0` | Representa el tipo de formato automático. |
| Custom | `2` | Representa un tipo de formato personalizado. |
| None | `1` | Representa el tipo de formato ninguno. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class FormattingTypeDemo
    {
        public static void FormattingTypeExample()
        {
            // Instanciar un objeto Workbook
            Workbook workbook = new Workbook();
            
            // Añadiendo una nueva hoja de cálculo al objeto Workbook
            int sheetIndex = workbook.Worksheets.Add();
            
            // Obteniendo la referencia de la hoja de cálculo recién añadida pasando su índice de hoja
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Agregar valores de muestra a celdas
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            
            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            
            // Accediendo a la instancia del gráfico recién agregado
            Chart chart = worksheet.Charts[chartIndex];
            
            // Añadiendo NSeries (fuente de datos del gráfico) al gráfico desde la celda "A1" hasta "B3"
            chart.NSeries.Add("A1:B3", true);
            
            // Estableciendo el color de primer plano del área de trazado
            chart.PlotArea.Area.ForegroundColor = Color.Blue;
            chart.PlotArea.Area.Formatting = FormattingType.Custom;
            
            // Estableciendo el color de primer plano del área del gráfico
            chart.ChartArea.Area.ForegroundColor = Color.Yellow;
            chart.ChartArea.Area.Formatting = FormattingType.Automatic;
            
            // Estableciendo el color de primer plano del área de la 1ª serie NSeries
            chart.NSeries[0].Area.ForegroundColor = Color.Red;
            chart.NSeries[0].Area.Formatting = FormattingType.None;
            
            // Estableciendo el color de primer plano del área del punto de la 1ª serie NSeries
            chart.NSeries[0].Points[0].Area.ForegroundColor = Color.Cyan;
            chart.NSeries[0].Points[0].Area.Formatting = FormattingType.Custom;
            
            // Guardando el archivo Excel
            workbook.Save("FormattingTypeExample.xlsx");
            workbook.Save("FormattingTypeExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


