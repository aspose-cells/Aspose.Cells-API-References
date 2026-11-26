---
title: "Area.InvertIfNegative"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Area. Si la propiedad es verdadera y el valor del punto del gráfico es un número negativo, el color de primer plano y el color de fondo se intercambiarán"
type: docs
url: /es/net/aspose.cells.drawing/area/invertifnegative/
---
## Area.InvertIfNegative property

Si la propiedad es verdadera y el valor del punto del gráfico es un número negativo, el color de primer plano y el color de fondo se intercambiarán.

```csharp
public bool InvertIfNegative { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AreaPropertyInvertIfNegativeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra con valor negativo
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(-100);
            worksheet.Cells["A3"].PutValue(150);
            
            // Agregar gráfico de columnas
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Agregar series de datos y configurar las propiedades del área
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries[0].Area.InvertIfNegative = true;
            chart.NSeries[0].Area.ForegroundColor = Color.Red;
            chart.NSeries[0].Area.BackgroundColor = Color.Yellow;
            
            workbook.Save("AreaPropertyInvertIfNegativeDemo.xls");
        }
    }
}
```

### Ver también

* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


