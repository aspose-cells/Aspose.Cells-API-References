---
title: "PivotOptions.DropZoneSeries"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotOptions. Especifica si un control para cada campo de PivotTable en el eje de columnas de la tabla dinámica de origen aparece en el gráfico cuando dropZonesVisible está configurado como verdadero"
type: docs
url: /es/net/aspose.cells.charts/pivotoptions/dropzoneseries/
---
## PivotOptions.DropZoneSeries property

Especifica si un control para cada campo de PivotTable en el eje de columnas de la PivotTable de origen aparece en el gráfico cuando dropZonesVisible está configurado a true.

```csharp
public bool DropZoneSeries { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PivotOptionsPropertyDropZoneSeriesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo y obtener la primera hoja
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            sheet.Cells["A1"].PutValue("Fruit");
            sheet.Cells["B1"].PutValue("Quantity");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["B3"].PutValue(5);
            sheet.Cells["A4"].PutValue("Banana");
            sheet.Cells["B4"].PutValue(7);

            // Añade un gráfico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = sheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("A1:B4", true);
            
            // Obtener opciones de tabla dinámica del gráfico
            PivotOptions options = chart.PivotOptions;
            
            // Demostrar la propiedad DropZoneSeries
            Console.WriteLine("Original DropZoneSeries value: " + options.DropZoneSeries);
            options.DropZoneSeries = true;
            Console.WriteLine("Modified DropZoneSeries value: " + options.DropZoneSeries);
            
            // Guarda el libro de trabajo
            workbook.Save("PivotOptionsPropertyDropZoneSeriesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


