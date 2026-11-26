---
title: "FillFormat.GradientFill"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FillFormat. Obtiene el objeto GradientFill"
type: docs
url: /es/net/aspose.cells.drawing/fillformat/gradientfill/
---
## FillFormat.GradientFill property

Obtiene el objeto `GradientFill`.

```csharp
public GradientFill GradientFill { get; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyGradientFillDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Proporciona algunos datos para un gráfico
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico de columnas
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Accede al formato de relleno del área de la primera serie
                FillFormat fillFormat = chart.NSeries[0].Area.FillFormat;

                // Aplica un degradado de dos colores a la serie
                fillFormat.SetTwoColorGradient(Color.Red, Color.Blue,
                                               GradientStyleType.Horizontal, 2);

                // Recupera el objeto GradientFill (propiedad de solo lectura)
                GradientFill gradientFill = fillFormat.GradientFill;

                // Muestra alguna información sobre el relleno degradado
                Console.WriteLine("GradientFill details:");
                Console.WriteLine($"  FillType      : {gradientFill.FillType}");
                Console.WriteLine($"  DirectionType: {gradientFill.DirectionType}");
                Console.WriteLine($"  Angle         : {gradientFill.Angle}");

                // Opcionalmente modifica el ángulo del degradado usando el accesor set
                gradientFill.Angle = 45.0f;
                Console.WriteLine($"  New Angle set to: {gradientFill.Angle}");

                // Guarda el libro de trabajo
                workbook.Save("FillFormatGradientFillDemo.xlsx");
                Console.WriteLine("Workbook saved as FillFormatGradientFillDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [GradientFill](../../gradientfill/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


