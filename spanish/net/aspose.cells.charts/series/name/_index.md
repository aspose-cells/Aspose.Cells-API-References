---
title: "Series.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Obtiene o establece el nombre de la serie de datos"
type: docs
url: /es/net/aspose.cells.charts/series/name/
---
## Series.Name property

Obtiene o establece el nombre de la serie de datos.

```csharp
public string Name { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Series Name");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["C2"].PutValue(30);
            
            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Agregar series al gráfico
            chart.NSeries.Add("A2:C2", true);
            
            // Demostrar el uso de la propiedad Name
            // 1. Nombre de referencia a una celda
            chart.NSeries[0].Name = "=A1";
            
            // 2. Establecer una cadena como nombre
            chart.NSeries[0].Name = "First Series";
            
            // Guarda el libro de trabajo
            workbook.Save("SeriesPropertyNameDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


