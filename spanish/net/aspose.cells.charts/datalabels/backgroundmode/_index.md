---
title: "DataLabels.BackgroundMode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataLabels. Obtiene y establece el modo de visualización del fondo"
type: docs
url: /es/net/aspose.cells.charts/datalabels/backgroundmode/
---
## DataLabels.BackgroundMode property

Obtiene y establece el modo de visualización del fondo

```csharp
public BackgroundMode BackgroundMode { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyBackgroundModeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(5);

            // Crear un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", true);

            // Obtener etiquetas de datos
            Aspose.Cells.Charts.DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;

            // Demostrar la propiedad BackgroundMode
            dataLabels.BackgroundMode = BackgroundMode.Automatic; // Automatic background
            Console.WriteLine("BackgroundMode set to Automatic");

            // Guarda el libro de trabajo
            workbook.Save("DataLabelsBackgroundModeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [BackgroundMode](../../backgroundmode/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


