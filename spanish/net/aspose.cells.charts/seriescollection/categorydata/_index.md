---
title: "SeriesCollection.CategoryData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SeriesCollection. Obtiene o establece el rango de valores del eje de categoría. Puede ser un rango de celdas como d1e10 o una secuencia de valores como 26810"
type: docs
url: /es/net/aspose.cells.charts/seriescollection/categorydata/
---
## SeriesCollection.CategoryData property

Obtiene o establece el rango de valores del eje de categoría. Puede ser un rango de celdas (como "d1:e10") o una secuencia de valores (como "{2,6,8,10}").

```csharp
public string CategoryData { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionPropertyCategoryDataDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue("Cat " + (i - 1));
                worksheet.Cells["B" + i].PutValue(i * 10);
            }
            
            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("=Sheet1!$B$2:$B$10", true);
            chart.NSeries.CategoryData = "=Sheet1!$A$2:$A$10";
            
            // Guarda el libro de trabajo
            workbook.Save("CategoryDataDemo.xlsx");
            
            // Verificar la propiedad CategoryData
            Console.WriteLine("Chart CategoryData: " + chart.NSeries.CategoryData);
        }
    }
}
```

### Ver también

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


