---
title: "Chart.CategoryAxis"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad del gráfico. Obtiene el eje X del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chart/categoryaxis/
---
## Chart.CategoryAxis property

Obtiene el eje X del gráfico.

```csharp
public Axis CategoryAxis { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyCategoryAxisDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico de columnas
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Acceder y modificar las propiedades de CategoryAxis
            chart.CategoryAxis.CategoryType = CategoryType.CategoryScale;
            chart.CategoryAxis.Title.Text = "Sample Categories";
            chart.CategoryAxis.Title.Font.Size = 12;

            // Guarda el libro de trabajo
            workbook.Save("CategoryAxisDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


