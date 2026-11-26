---
title: "ImageOrPrintOptions.WarningCallback"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Obtiene o establece la devolución de llamada de advertencia"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/warningcallback/
---
## ImageOrPrintOptions.WarningCallback property

Obtiene o establece la devolución de llamada de advertencia.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar contenido que generará una advertencia durante el renderizado
            worksheet.Cells["A1"].PutValue("This text uses a non-existent font");
            Style style = workbook.CreateStyle();
            style.Font.Name = "NonExistentFont";
            worksheet.Cells["A1"].SetStyle(style);

            // Crear una instancia de ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // Mostrar el valor inicial de WarningCallback
            Console.WriteLine("Current WarningCallback value: " + options.WarningCallback);

            // Crear y asignar una devolución de llamada de advertencia personalizada
            var warningCallback = new RenderingWarningCallback();
            options.WarningCallback = warningCallback;

            // Crear SheetRender para demostrar la devolución de llamada durante el renderizado
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "output_image.png");

            // Verificar si se capturaron advertencias
            Console.WriteLine($"Total warnings captured: {warningCallback.WarningCount}");
        }
    }

    // Implementación personalizada de devolución de llamada para manejar advertencias de renderizado
    public class RenderingWarningCallback : IWarningCallback
    {
        public int WarningCount { get; private set; }

        public void Warning(WarningInfo warningInfo)
        {
            // Manejar advertencias de sustitución de fuentes
            if (warningInfo.WarningType == WarningType.FontSubstitution)
            {
                Console.WriteLine($"Font substitution warning: {warningInfo.Description}");
                WarningCount++;
            }
        }
    }
}
```

### Ver también

* interface [IWarningCallback](../../../aspose.cells/iwarningcallback/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


