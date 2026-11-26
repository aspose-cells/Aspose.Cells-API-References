---
title: "ChartFrame.IsDefaultPosBeSet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartFrame. Indica si la posición predeterminada DefaultX DefaultY DefaultWidth y DefaultHeight está establecida"
type: docs
url: /es/net/aspose.cells.charts/chartframe/isdefaultposbeset/
---
## ChartFrame.IsDefaultPosBeSet property

Indica si la posición predeterminada (DefaultX, DefaultY, DefaultWidth y DefaultHeight) está establecida.

```csharp
public bool IsDefaultPosBeSet { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyIsDefaultPosBeSetDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Bar, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Acceder a las etiquetas de datos
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            
            // Demostrar la propiedad IsDefaultPosBeSet
            Console.WriteLine("IsDefaultPosBeSet before setting position: " + dataLabels.IsDefaultPosBeSet);
            
            // Cambiar la posición y comprobar la propiedad nuevamente
            dataLabels.Position = LabelPositionType.InsideBase;
            Console.WriteLine("IsDefaultPosBeSet after setting position: " + dataLabels.IsDefaultPosBeSet);
        }
    }
}
```

### Ver también

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


