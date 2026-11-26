---
title: "ImageOrPrintOptions.ChartImageType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ImageOrPrintOptions property. Indique el tipo de imagen del gráfico al convertir. valor predeterminado PNG"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/chartimagetype/
---
## ImageOrPrintOptions.ChartImageType property

Indique el tipo de imagen del gráfico al convertir. valor predeterminado: PNG.

```csharp
[Obsolete("Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ImageFormat ChartImageType { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, Chart y Shape siempre se renderizan como elementos vectoriales (p. ej., punto, línea) para mejorar la calidad de renderizado. Esta propiedad será eliminada 12 meses después desde junio de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertyChartImageTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Añade una hoja de cálculo con un gráfico
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = 10;
            worksheet.Cells["A3"].Value = 20;
            worksheet.Cells["A4"].Value = 30;

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A2:A4", true);

            try
            {
                // Crear una instancia de ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Muestra el valor actual de ChartImageType
                Console.WriteLine("Current ChartImageType: " + options.ImageType);

                // Establece un tipo de imagen diferente para la renderización del gráfico
                options.ImageType = ImageType.Png;
                Console.WriteLine("ChartImageType set to: " + options.ImageType);

                // Crea un SheetRender para demostrar el efecto de la propiedad
                SheetRender renderer = new SheetRender(worksheet, options);

                // Renderiza el gráfico a un flujo de memoria
                MemoryStream stream = new MemoryStream();
                renderer.ToImage(0, stream);

                Console.WriteLine("Chart rendered successfully with ChartImageType: " + options.ImageType);
                Console.WriteLine("Image size: " + stream.Length + " bytes");

                // Guarda el libro de trabajo
                workbook.Save("ChartImageTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


