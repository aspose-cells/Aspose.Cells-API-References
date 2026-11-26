---
title: "FillFormat.GradientDegree"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FillFormat. Devuelve el grado de degradado para el relleno especificado. Solo se aplica a Excel 2007"
type: docs
url: /es/net/aspose.cells.drawing/fillformat/gradientdegree/
---
## FillFormat.GradientDegree property

Devuelve el grado de degradado para el relleno especificado. Solo se aplica a Excel 2007.

```csharp
public double GradientDegree { get; }
```

### Observaciones

Solo puede ser un valor de 0.0 (oscuro) a 1.0 (claro).

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyGradientDegreeDemo
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
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Establecer relleno de degradado para la primera serie
            Aspose.Cells.Drawing.FillFormat fillFormat = chart.NSeries[0].Area.FillFormat;
            fillFormat.SetTwoColorGradient(Color.Red, Color.Blue, Aspose.Cells.Drawing.GradientStyleType.Horizontal, 2);
            
            // Mostrar el grado de degradado
            Console.WriteLine("Gradient Degree: " + fillFormat.GradientDegree);

            // Guarda el libro de trabajo
            workbook.Save("GradientDegreeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


