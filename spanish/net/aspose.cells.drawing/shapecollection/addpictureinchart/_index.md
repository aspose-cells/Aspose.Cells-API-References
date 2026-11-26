---
title: "ShapeCollection.AddPictureInChart"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Agrega una imagen al gráfico"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addpictureinchart/
---
## ShapeCollection.AddPictureInChart method

Agrega una imagen al gráfico.

```csharp
public Picture AddPictureInChart(int top, int left, Stream stream, int widthScale, int heightScale)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| superior | Int32 | Representa el desplazamiento vertical de la forma desde la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |
| izquierda | Int32 | Representa el desplazamiento horizontal de la forma desde la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |
| stream | Stream | Objeto Stream que contiene los datos de la imagen. |
| widthScale | Int32 | Escala del ancho de la imagen, un porcentaje. |
| heightScale | Int32 | Escala de la altura de la imagen, un porcentaje. |

### Valor de retorno

Devuelve un objeto Picture.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts; // Added this using directive
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ShapeCollectionMethodAddPictureInChartWithInt32Int32StreamInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 15, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries.CategoryData = "B1:B3";

            // Crea un flujo de memoria con datos de imagen
            byte[] imageData = File.ReadAllBytes("example.jpg");
            MemoryStream stream = new MemoryStream(imageData);

            try
            {
                // Llama a AddPictureInChart con los parámetros (Int32, Int32, Stream, Int32, Int32)
                Picture picture = chart.Shapes.AddPictureInChart(100, 100, stream, 50, 50);
                
                Console.WriteLine("Picture added to chart successfully. Original dimensions: " + 
                    $"{picture.OriginalWidth}x{picture.OriginalHeight}");
                
                // Guarda el libro de trabajo
                workbook.Save("AddPictureInChartDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddPictureInChart method: {ex.Message}");
            }
            finally
            {
                stream.Dispose();
            }
        }
    }
}
```

### Ver también

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


