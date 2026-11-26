---
title: "DataLabels.IsTextWrapped"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataLabels. Obtiene o establece un valor que indica si el texto está ajustado"
type: docs
url: /es/net/aspose.cells.charts/datalabels/istextwrapped/
---
## DataLabels.IsTextWrapped property

Obtiene o establece un valor que indica si el texto está ajustado.

```csharp
public override bool IsTextWrapped { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyIsTextWrappedDemo
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
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(85);
            worksheet.Cells["B4"].PutValue(65);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Acceder a las etiquetas de datos
            Aspose.Cells.Charts.DataLabels labels = chart.NSeries[0].DataLabels;
            
            // Mostrar etiquetas de datos
            labels.ShowValue = true;
            
            // Demostrar la propiedad IsTextWrapped
            Console.WriteLine("Before setting IsTextWrapped: " + labels.IsTextWrapped);
            labels.IsTextWrapped = true;
            Console.WriteLine("After setting IsTextWrapped: " + labels.IsTextWrapped);

            // Guarda el libro de trabajo
            workbook.Save("DataLabels_IsTextWrapped_Demo.xlsx");
        }
    }
}
```

### Ver también

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


