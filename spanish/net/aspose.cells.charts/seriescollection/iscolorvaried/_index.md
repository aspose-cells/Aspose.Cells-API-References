---
title: "SeriesCollection.IsColorVaried"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SeriesCollection. Representa si el color de los puntos es variado"
type: docs
url: /es/net/aspose.cells.charts/seriescollection/iscolorvaried/
---
## SeriesCollection.IsColorVaried property

Representa si el color de los puntos varía.

```csharp
public bool IsColorVaried { get; set; }
```

### Observaciones

Solo funciona para gráficos de pastel o cuando hay una sola serie.

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionPropertyIsColorVariedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Datos de ejemplo
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Region");
            cells["A2"].PutValue("France");
            cells["A3"].PutValue("Germany");
            cells["A4"].PutValue("England");
            cells["A5"].PutValue("USA");
            cells["B1"].PutValue("Sales");
            cells["B2"].PutValue(70000);
            cells["B3"].PutValue(55000);
            cells["B4"].PutValue(30000);
            cells["B5"].PutValue(85000);

            // Crear gráfico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            
            // Agregar serie
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";
            
            // Establecer la propiedad IsColorVaried
            chart.NSeries.IsColorVaried = true;
            
            // Guarda el libro de trabajo
            workbook.Save("SeriesCollectionPropertyIsColorVariedDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


