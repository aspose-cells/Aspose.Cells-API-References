---
title: "DataLabels.ShowCategoryName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataLabels. Representa el comportamiento de visualización del nombre de categoría de la etiqueta de datos de un gráfico especificado. Verdadero para mostrar el nombre de categoría en las etiquetas de datos del gráfico. Falso para ocultar"
type: docs
url: /es/net/aspose.cells.charts/datalabels/showcategoryname/
---
## DataLabels.ShowCategoryName property

Representa el comportamiento de visualización del nombre de categoría de la etiqueta de datos de un gráfico especificado. True para mostrar el nombre de categoría en las etiquetas de datos de un gráfico. False para ocultarlo.

```csharp
public bool ShowCategoryName { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowCategoryNameDemo
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

            // Agregar un gráfico de columnas
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Habilitar etiquetas de datos y establecer propiedades
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;
            dataLabels.ShowCategoryName = true;
            dataLabels.SeparatorType = DataLabelsSeparatorType.Semicolon;

            // Guarda el libro de trabajo
            workbook.Save("DataLabelsShowCategoryNameDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


