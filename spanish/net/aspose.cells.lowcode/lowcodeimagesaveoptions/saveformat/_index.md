---
title: "LowCodeImageSaveOptions.SaveFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LowCodeImageSaveOptions. Obtiene o establece el formato de guardado"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodeimagesaveoptions/saveformat/
---
## LowCodeImageSaveOptions.SaveFormat property

Obtiene o establece el formato de guardado.

```csharp
public override SaveFormat SaveFormat { get; set; }
```

### Observaciones

Si se ha especificado [`ImageOptions`](../imageoptions/), establecer esta propiedad también cambiará el valor de [`ImageType`](../../../aspose.cells.rendering/imageorprintoptions/imagetype/) de la misma.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeImageSaveOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells LowCode Image SaveFormat Demo");

            // Inicializar LowCodeImageSaveOptions con valores predeterminados
            LowCodeImageSaveOptions options = new LowCodeImageSaveOptions();
            
            // Mostrar SaveFormat inicial (el predeterminado es Png)
            Console.WriteLine("Initial SaveFormat: " + options.SaveFormat);

            // Configurar para salida JPEG
            options.SaveFormat = SaveFormat.Jpg;
            options.ImageOptions = new ImageOrPrintOptions
            {
                Quality = 85,
                OnePagePerSheet = true,
                ImageType = ImageType.Jpeg
            };
            SaveWorksheetAsImage(worksheet, options, "output_initial.jpg");

            // Cambiar al formato PNG y guardar de nuevo
            options.SaveFormat = SaveFormat.Png;
            options.ImageOptions.ImageType = ImageType.Png;
            Console.WriteLine("\nModified SaveFormat: " + options.SaveFormat);
            SaveWorksheetAsImage(worksheet, options, "output_modified.png");
        }

        private static void SaveWorksheetAsImage(Worksheet worksheet, LowCodeImageSaveOptions options, string fileName)
        {
            // Renderizar hoja de cálculo usando opciones configuradas
            SheetRender renderer = new SheetRender(worksheet, options.ImageOptions);
            renderer.ToImage(0, fileName);
            Console.WriteLine($"Saved: {fileName}");
        }
    }
}
```

### Ver también

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodeImageSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


