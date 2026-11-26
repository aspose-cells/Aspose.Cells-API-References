---
title: "SeriesCollection.SecondCategoryData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SeriesCollection. Obtiene o establece el rango de valores del segundo eje de categoría. Puede ser un rango de celdas como d1e10 o una secuencia de valores como 26810. Solo tiene efecto cuando algunas series se trazan en el segundo eje"
type: docs
url: /es/net/aspose.cells.charts/seriescollection/secondcategorydata/
---
## SeriesCollection.SecondCategoryData property

Obtiene o establece el rango de valores del segundo eje de categoría. Puede ser un rango de celdas (como "d1:e10"), o una secuencia de valores (como "{2,6,8,10}"). Solo tiene efecto cuando algunas series se trazaron en el segundo eje.

```csharp
public string SecondCategoryData { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionPropertySecondCategoryDataDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Primary Categories");
            worksheet.Cells["A2"].PutValue("Cat1");
            worksheet.Cells["A3"].PutValue("Cat2");
            worksheet.Cells["A4"].PutValue("Cat3");
            
            worksheet.Cells["B1"].PutValue("Secondary Categories");
            worksheet.Cells["B2"].PutValue("SubCat1");
            worksheet.Cells["B3"].PutValue("SubCat2");
            worksheet.Cells["B4"].PutValue("SubCat3");
            
            worksheet.Cells["C1"].PutValue("Values");
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(20);
            worksheet.Cells["C4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer datos de la serie
            chart.NSeries.Add("C2:C4", true);
            
            // Establecer datos de la categoría primaria
            chart.NSeries.CategoryData = "A2:A4";
            
            // Establecer datos de la categoría secundaria
            chart.NSeries.SecondCategoryData = "B2:B4";

            // Guarda el libro de trabajo
            workbook.Save("SecondCategoryDataDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


