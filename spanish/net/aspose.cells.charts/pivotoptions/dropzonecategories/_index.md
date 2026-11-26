---
title: "PivotOptions.DropZoneCategories"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotOptions. Especifica si un control para cada campo de PivotTable en el eje de filas de la tabla dinámica de origen aparece en el gráfico cuando dropZonesVisible está configurado como verdadero"
type: docs
url: /es/net/aspose.cells.charts/pivotoptions/dropzonecategories/
---
## PivotOptions.DropZoneCategories property

Especifica si un control para cada campo de PivotTable en el eje de filas de la PivotTable de origen aparece en el gráfico cuando dropZonesVisible está configurado a true.

```csharp
public bool DropZoneCategories { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PivotOptionsPropertyDropZoneCategoriesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo y algunos datos de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            
            // Agregar un gráfico que use datos de tabla dinámica
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Acceder a las opciones de tabla dinámica del gráfico
            PivotOptions options = chart.PivotOptions;
            
            // Demostrar la propiedad DropZoneCategories
            options.DropZoneCategories = true;
            Console.WriteLine("DropZoneCategories enabled: " + options.DropZoneCategories);
            
            // Guarda el libro de trabajo
            workbook.Save("PivotOptionsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


