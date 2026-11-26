---
title: "Axis.CategoryType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Axis. Representa el tipo del eje de categoría"
type: docs
url: /es/net/aspose.cells.charts/axis/categorytype/
---
## Axis.CategoryType property

Representa el tipo del eje de categoría.

```csharp
public CategoryType CategoryType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyCategoryTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue("Cat " + (i - 1));
                sheet.Cells["B" + i].PutValue(i * 10);
            }

            // Añade un gráfico
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 2, 25, 11);
            Chart chart = sheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("=Sheet1!$A$1:$B$10", true);

            // Demostrar la propiedad CategoryType
            chart.CategoryAxis.CategoryType = Aspose.Cells.Charts.CategoryType.AutomaticScale;
            Console.WriteLine("CategoryType set to AutomaticScale");

            // Guarda el libro de trabajo
            workbook.Save("AxisPropertyCategoryTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* enum [CategoryType](../../categorytype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


