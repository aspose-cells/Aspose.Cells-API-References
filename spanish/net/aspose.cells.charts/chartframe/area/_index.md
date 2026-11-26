---
title: "ChartFrame.Area"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartFrame. Obtiene el área"
type: docs
url: /es/net/aspose.cells.charts/chartframe/area/
---
## ChartFrame.Area property

Obtiene el `area`.

```csharp
public virtual Area Area { get; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyAreaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Acceder al área del gráfico
            ChartArea chartArea = chart.ChartArea;
            
            // Demostrar la funcionalidad de la propiedad Area
            Area area = chartArea.Area;
            Console.WriteLine("Original Formatting: " + area.Formatting);
            
            // Modificar propiedades del área
            area.Formatting = FormattingType.Custom;
            area.BackgroundColor = Color.LightBlue;
            area.ForegroundColor = Color.DarkBlue;
            area.Transparency = 0.3;
            area.InvertIfNegative = true;

            // Guarda el libro de trabajo
            workbook.Save("ChartFramePropertyAreaDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Area](../../../aspose.cells.drawing/area/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


