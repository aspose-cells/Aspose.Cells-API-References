---
title: "Chart.SecondCategoryAxis"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad del gráfico. Obtiene el segundo eje X del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chart/secondcategoryaxis/
---
## Chart.SecondCategoryAxis property

Obtiene el segundo eje X del gráfico.

```csharp
public Axis SecondCategoryAxis { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertySecondCategoryAxisDemo
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
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(15);
            worksheet.Cells["C3"].PutValue(25);
            worksheet.Cells["C4"].PutValue(35);

            // Agregar un gráfico con eje secundario
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Agregar series al gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.Add("C2:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Habilitar eje de categoría secundario
            chart.SecondCategoryAxis.IsVisible = true;
            chart.SecondCategoryAxis.Title.Text = "Secondary Category Axis";
            
            // Establecer algunas propiedades del eje de categoría secundario
            chart.SecondCategoryAxis.MajorTickMark = TickMarkType.Cross;
            chart.SecondCategoryAxis.MinorTickMark = TickMarkType.Outside;
            chart.SecondCategoryAxis.TickLabelPosition = TickLabelPositionType.NextToAxis;

            // Guarda el libro de trabajo
            workbook.Save("SecondCategoryAxisDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


