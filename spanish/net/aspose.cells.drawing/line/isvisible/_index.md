---
title: "Line.IsVisible"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Line. Representa si la línea es visible"
type: docs
url: /es/net/aspose.cells.drawing/line/isvisible/
---
## Line.IsVisible property

Representa si la línea es visible.

```csharp
public bool IsVisible { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LinePropertyIsVisibleDemo
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
            
            // Acceder a las líneas de cuadrícula principales y establecer la visibilidad
            chart.CategoryAxis.MajorGridLines.IsVisible = true;
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            // Verificar la visibilidad
            Console.WriteLine("Major Gridlines Visible: " + chart.CategoryAxis.MajorGridLines.IsVisible);
        }
    }
}
```

### Ver también

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


