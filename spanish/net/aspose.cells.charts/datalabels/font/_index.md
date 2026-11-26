---
title: "DataLabels.Font"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataLabels. Obtiene la fuente de las DataLabels"
type: docs
url: /es/net/aspose.cells.charts/datalabels/font/
---
## DataLabels.Font property

Obtiene la fuente de los DataLabels;

```csharp
public override Font Font { get; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyFontDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Habilitar etiquetas de datos
            Aspose.Cells.Charts.DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;

            // Establecer propiedades de fuente
            dataLabels.Font.Color = Color.Red;
            dataLabels.Font.Size = 14;
            dataLabels.Font.IsBold = true;
            dataLabels.Font.Name = "Arial";

            // Guarda el libro de trabajo
            workbook.Save("DataLabelsFontDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Font](../../../aspose.cells/font/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


