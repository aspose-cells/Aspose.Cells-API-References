---
title: "Enumeración BackgroundMode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Charts.BackgroundMode. Representa el modo de visualización del fondo"
type: docs
url: /es/net/aspose.cells.charts/backgroundmode/
---
## BackgroundMode enumeration

Representa el modo de visualización del fondo.

```csharp
public enum BackgroundMode
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Automatic | `0` | Automático |
| Opaque | `1` | Opaco |
| Transparent | `2` | Transparente |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class BackgroundModeDemo
    {
        public static void BackgroundModeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Obtenga la referencia de la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos de ejemplo a las celdas
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            
            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Agrega NSeries (fuente de datos del gráfico) al gráfico que abarca desde la celda "A1" hasta "B3"
            chart.NSeries.Add("A1:B3", true);
            
            // Acceder al área del gráfico
            ChartArea chartArea = chart.ChartArea;

            // Establecer el color de primer plano del área del gráfico
            chartArea.Area.ForegroundColor = Color.Yellow;

            // Establecer el modo de fondo del área del gráfico
            chartArea.BackgroundMode = BackgroundMode.Opaque;
            chartArea.Area.Transparency = 0.8;           
            
            
            // Establecer la sombra del área del gráfico
            chartArea.Shadow = true;
            
            // Guarda el libro de trabajo
            workbook.Save("BackgroundModeExample.xlsx");
            workbook.Save("BackgroundModeExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


