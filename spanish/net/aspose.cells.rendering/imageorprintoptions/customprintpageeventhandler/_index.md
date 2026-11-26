---
title: "ImageOrPrintOptions.CustomPrintPageEventHandler"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. El cliente puede enviar una salida especial a la impresora al imprimir cada página usando este EventHandler"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler/
---
## ImageOrPrintOptions.CustomPrintPageEventHandler property

El cliente puede enviar una salida especial a la impresora al imprimir cada página usando este EventHandler

```csharp
public PrintPageEventHandler CustomPrintPageEventHandler { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyCustomPrintPageEventHandlerDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].Value = "Sample Data for Printing";
            worksheet.Cells["A2"].Value = "This demonstrates printing options";

            try
            {
                // Crear una instancia de ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Configurar opciones de impresión
                options.PrintWithStatusDialog = true;
                options.HorizontalResolution = 300;
                options.VerticalResolution = 300;

                // Mostrar las opciones de impresión actuales
                Console.WriteLine($"PrintWithStatusDialog: {options.PrintWithStatusDialog}");
                Console.WriteLine($"HorizontalResolution: {options.HorizontalResolution}");
                Console.WriteLine($"VerticalResolution: {options.VerticalResolution}");

                // Crear un SheetRender para demostrar la impresión
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Renderizar a imagen para demostrar la impresión
                sheetRender.ToImage(0, "output.png");
                Console.WriteLine("Rendering completed successfully.");
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


