---
title: "DataLabels.IsAutoText"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataLabels. Indica que el texto se genera automáticamente"
type: docs
url: /es/net/aspose.cells.charts/datalabels/isautotext/
---
## DataLabels.IsAutoText property

Indica que el texto se genera automáticamente.

```csharp
public override bool IsAutoText { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyIsAutoTextDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Habilitar etiquetas de datos
            foreach (Series series in chart.NSeries)
            {
                series.DataLabels.ShowValue = true;
                
                // Demostrar la propiedad IsAutoText
                foreach (ChartPoint point in series.Points)
                {
                    Console.WriteLine("IsAutoText before setting: " + point.DataLabels.IsAutoText);
                    point.DataLabels.IsAutoText = false;
                    point.DataLabels.Text = "Custom " + point.YValue;
                    Console.WriteLine("IsAutoText after setting: " + point.DataLabels.IsAutoText);
                    Console.WriteLine("DataLabel Text: " + point.DataLabels.Text);
                }
            }
            
            // Guarda el libro de trabajo
            workbook.Save("DataLabelsIsAutoTextDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


