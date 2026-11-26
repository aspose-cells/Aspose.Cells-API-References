---
title: "SeriesLayoutProperties.ShowMeanLine"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SeriesLayoutProperties. Indica si se muestra la línea que conecta todos los puntos de media"
type: docs
url: /es/net/aspose.cells.charts/serieslayoutproperties/showmeanline/
---
## SeriesLayoutProperties.ShowMeanLine property

Indica si se muestra la línea que conecta todos los puntos de media.

```csharp
public bool ShowMeanLine { get; set; }
```

### Observaciones

Solo funciona para el gráfico BoxWhisker.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyShowMeanLineDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para el gráfico de caja y bigotes
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(40);
            worksheet.Cells["A4"].PutValue(25);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["A6"].PutValue(115);
            worksheet.Cells["A7"].PutValue(65.666);

            // Agregar un gráfico de caja y bigotes
            int chartIndex = worksheet.Charts.Add(ChartType.BoxWhisker, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Agregar series al gráfico
            chart.NSeries.Add("A1:A7", true);

            // Obtener la primera serie
            Series series = chart.NSeries[0];

            // Acceder a las propiedades de diseño
            SeriesLayoutProperties layout = series.LayoutProperties;

            // Demostrar la propiedad ShowMeanLine
            Console.WriteLine("Default ShowMeanLine value: " + layout.ShowMeanLine);
            
            // Establecer ShowMeanLine en true
            layout.ShowMeanLine = true;
            Console.WriteLine("After setting ShowMeanLine to true: " + layout.ShowMeanLine);

            // Guarda el libro de trabajo
            workbook.Save("BoxWhiskerChart_ShowMeanLineDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


