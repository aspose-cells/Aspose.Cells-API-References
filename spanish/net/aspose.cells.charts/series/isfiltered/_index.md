---
title: "Series.IsFiltered"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Indica si la serie está seleccionada o filtrada. True indica que esta serie está filtrada y no se mostrará en el gráfico"
type: docs
url: /es/net/aspose.cells.charts/series/isfiltered/
---
## Series.IsFiltered property

Indica si la serie está seleccionada o filtrada. True indica que esta serie está filtrada y no se mostrará en el gráfico.

```csharp
public bool IsFiltered { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyIsFilteredDemo
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
            worksheet.Cells["A5"].PutValue("D");
            
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["C2"].PutValue(15);
            worksheet.Cells["C3"].PutValue(25);
            worksheet.Cells["C4"].PutValue(35);
            worksheet.Cells["C5"].PutValue(45);
            
            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.Add("C2:C5", true);
            chart.NSeries.CategoryData = "A2:A5";
            
            // Demostrar la propiedad IsFiltered
            Console.WriteLine("Initial Series Count: " + chart.NSeries.Count);
            
            // Filtrar la primera serie
            chart.NSeries[0].IsFiltered = true;
            Console.WriteLine("After filtering first series: " + chart.NSeries.Count);
            
            // Filtrar la segunda serie
            chart.NSeries[0].IsFiltered = true;
            Console.WriteLine("After filtering second series: " + chart.NSeries.Count);
            
            // Guarda el libro de trabajo
            workbook.Save("SeriesFilteredDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


