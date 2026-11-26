---
title: "ImageOrPrintOptions.PageSavingCallback"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Controlar/Indicar el progreso del proceso de guardado de página"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/pagesavingcallback/
---
## ImageOrPrintOptions.PageSavingCallback property

Controlar/Indicar el progreso del proceso de guardado de la página.

```csharp
public IPageSavingCallback PageSavingCallback { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyPageSavingCallbackDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y rellenar datos
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo que abarcan varias páginas
            worksheet.Cells["A1"].PutValue("PageSavingCallback Demonstration");
            for (int i = 1; i <= 50; i++)
            {
                worksheet.Cells[$"A{i + 1}"].PutValue($"Data Row {i}");
            }

            // Configurar la configuración de página para generar varias páginas
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.PaperSize = PaperSizeType.PaperA4;
            pageSetup.Orientation = PageOrientationType.Portrait;
            pageSetup.FitToPagesWide = 1;
            pageSetup.FitToPagesTall = 0;

            // Inicializar ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionCCITT4
            };

            // Mostrar el estado inicial del callback
            Console.WriteLine($"Initial PageSavingCallback: {options.PageSavingCallback}");

            // Establecer el callback personalizado de guardado de página
            options.PageSavingCallback = new CustomPageSavingCallback();

            // Renderizar la hoja de cálculo a TIFF multipágina
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToTiff("output_with_callback.tiff");

            // Guardar el libro de trabajo como referencia
            workbook.Save("PageSavingCallbackDemo.xlsx");
        }

        private class CustomPageSavingCallback : IPageSavingCallback
        {
            public void PageStartSaving(PageStartSavingArgs args)
            {
                Console.WriteLine($"Processing page {args.PageIndex}");
                
                // Omitir la primera página (índice basado en 0)
                if (args.PageIndex == 0)
                {
                    args.IsToOutput = false;
                    Console.WriteLine("Skipping first page");
                }
            }

            public void PageEndSaving(PageEndSavingArgs args)
            {
                Console.WriteLine($"Completed processing page {args.PageIndex}");
            }
        }
    }
}
```

### Ver también

* interface [IPageSavingCallback](../../ipagesavingcallback/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


