---
title: "Axis.AxisBetweenCategories"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Axis. Representa si el eje de valores cruza el eje de categorías entre categorías"
type: docs
url: /es/net/aspose.cells.charts/axis/axisbetweencategories/
---
## Axis.AxisBetweenCategories property

Representa si el eje de valores cruza el eje de categoría entre categorías.

```csharp
public bool AxisBetweenCategories { get; set; }
```

### Observaciones

Esta propiedad se aplica solo a ejes de categorías, y no se aplica a gráficos 3D.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AxisPropertyAxisBetweenCategoriesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceda a la primera hoja de cálculo y agregue datos de muestra
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Categories");
            worksheet.Cells["B1"].PutValue("Values");
            
            for (int i = 1; i <= 5; i++)
            {
                worksheet.Cells[$"A{i+1}"].PutValue($"Category {i}");
                worksheet.Cells[$"B{i+1}"].PutValue(i * 10);
            }

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer datos del gráfico
            chart.NSeries.Add("B2:B6", true);
            chart.NSeries.CategoryData = "A2:A6";

            // Configurar eje de categorías
            Axis categoryAxis = chart.CategoryAxis;
            categoryAxis.AxisBetweenCategories = false; // Core property demonstration
            categoryAxis.TickLabels.RotationAngle = 45;

            // Guarda el libro de trabajo
            workbook.Save("AxisBetweenCategoriesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


