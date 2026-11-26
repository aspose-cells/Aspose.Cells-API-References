---
title: "Clase LowCodeImageSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.LowCode.LowCodeImageSaveOptions. Opciones para guardar imágenes de forma low code"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodeimagesaveoptions/
---
## LowCodeImageSaveOptions class

Opciones para guardar imágenes de forma low code.

```csharp
public class LowCodeImageSaveOptions : LowCodeSaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [LowCodeImageSaveOptions](lowcodeimagesaveoptions/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ImageOptions](../../aspose.cells.lowcode/lowcodeimagesaveoptions/imageoptions/) { get; set; } | Las opciones para renderizar imágenes. |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | Obtiene y establece el archivo (con ruta si es necesario) para guardar los datos generados. Al establecer esta propiedad con un valor distinto de null o cadena vacía, [`OutputStream`](../lowcodesaveoptions/outputstream/) será ignorado.(Hereda de [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | Obtiene y establece el Stream para escribir los datos generados. Al establecer esta propiedad con un valor distinto de null, [`OutputFile`](../lowcodesaveoptions/outputfile/) será ignorado.(Hereda de [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| override [SaveFormat](../../aspose.cells.lowcode/lowcodeimagesaveoptions/saveformat/) { get; set; } | Obtiene o establece el formato de guardado. |
| [SaveOptionsProvider](../../aspose.cells.lowcode/lowcodeimagesaveoptions/saveoptionsprovider/) { get; set; } | Proveedor de opciones de guardado para guardar imágenes generadas. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeClassLowCodeImageSaveOptionsDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Agregar datos de ejemplo a la hoja de cálculo
                worksheet.Cells["A1"].PutValue("LowCode Image Save Demo");
                worksheet.Cells["A2"].PutValue("This demonstrates LowCodeImageSaveOptions");

                // Crear una instancia de LowCodeImageSaveOptions
                LowCodeImageSaveOptions saveOptions = new LowCodeImageSaveOptions();

                // Establecer propiedades básicas
                saveOptions.SaveFormat = SaveFormat.Png;
                saveOptions.ImageOptions = new ImageOrPrintOptions();

                // Mostrar la configuración actual
                Console.WriteLine("SaveFormat: " + saveOptions.SaveFormat);
                Console.WriteLine("ImageOptions HorizontalResolution: " +
                    saveOptions.ImageOptions.HorizontalResolution);

                // Modificar algunas opciones de imagen
                saveOptions.ImageOptions.HorizontalResolution = 300;
                saveOptions.ImageOptions.VerticalResolution = 300;

                // Crear un proveedor simple de opciones de guardado
                saveOptions.SaveOptionsProvider = new SimpleSaveOptionsProvider();

                // Guardar la hoja de cálculo como una imagen
                SheetRender renderer = new SheetRender(worksheet, saveOptions.ImageOptions);
                renderer.ToImage(0, "LowCodeImageOutput.png");

                Console.WriteLine("Image saved successfully with LowCodeImageSaveOptions");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with LowCodeImageSaveOptions: {ex.Message}");
            }
        }
    }

    public class SimpleSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            return new LowCodeImageSaveOptions()
            {
                SaveFormat = SaveFormat.Png,
                ImageOptions = new ImageOrPrintOptions()
                {
                    HorizontalResolution = 300,
                    VerticalResolution = 300
                }
            };
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            Console.WriteLine("Finished saving part");
        }
    }
}
```

### Ver también

* class [LowCodeSaveOptions](../lowcodesaveoptions/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


