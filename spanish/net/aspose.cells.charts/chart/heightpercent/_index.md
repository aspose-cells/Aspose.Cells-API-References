---
title: "Chart.HeightPercent"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Chart. Devuelve o establece la altura de un gráfico 3D como un porcentaje del ancho del gráfico entre 5 y 500 por ciento"
type: docs
url: /es/net/aspose.cells.charts/chart/heightpercent/
---
## Chart.HeightPercent property

Devuelve o establece la altura de un gráfico 3-D como un porcentaje del ancho del gráfico (entre el 5 y el 500 por ciento).

```csharp
public int HeightPercent { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyHeightPercentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico de columnas 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Establecer la propiedad HeightPercent (controla la altura del gráfico 3D como porcentaje del ancho del gráfico)
            chart.HeightPercent = 150; // 150% of chart width

            // Guarda el libro de trabajo
            workbook.Save("ChartHeightPercentDemo.xlsx");

            Console.WriteLine("Chart with HeightPercent 150% created successfully.");
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


