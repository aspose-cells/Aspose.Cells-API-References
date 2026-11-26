---
title: "Legend.IsOverLay"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Legend. Obtiene o establece si se muestra la leyenda sin superponerse al gráfico"
type: docs
url: /es/net/aspose.cells.charts/legend/isoverlay/
---
## Legend.IsOverLay property

Obtiene o establece si se muestra la leyenda sin superponerse al gráfico.

```csharp
public bool IsOverLay { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendPropertyIsOverLayDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
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
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Establecer superposición de leyenda
            chart.Legend.IsOverLay = true;
            
            // Guarda el libro de trabajo
            workbook.Save("LegendOverlayDemo.xlsx");
            
            Console.WriteLine("Chart with overlay legend created successfully.");
        }
    }
}
```

### Ver también

* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


