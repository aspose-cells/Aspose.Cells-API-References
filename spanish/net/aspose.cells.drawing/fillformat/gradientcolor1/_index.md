---
title: "FillFormat.GradientColor1"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FillFormat. Devuelve el color de degradado 1 para el relleno especificado"
type: docs
url: /es/net/aspose.cells.drawing/fillformat/gradientcolor1/
---
## FillFormat.GradientColor1 property

Devuelve el color de degradado 1 para el relleno especificado.

```csharp
public Color GradientColor1 { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyGradientColor1Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Obtener el formato de relleno de la primera serie
            FillFormat fillFormat = chart.NSeries[0].Area.FillFormat;
            
            // Crear un relleno degradado usando los tipos de parámetros correctos
            fillFormat.SetTwoColorGradient(
                Color.Red, 
                Color.White, 
                GradientStyleType.Horizontal, 
                1); // Gradient variant must be integer (1-4)

            // Obtener y mostrar el color de degradado
            Color gradientColor1 = fillFormat.GradientColor1;
            Console.WriteLine("Gradient Color 1: " + gradientColor1);
            Console.WriteLine("Gradient Degree: " + fillFormat.GradientDegree);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


