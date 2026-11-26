---
title: "LowCodeImageSaveOptions.SaveOptionsProvider"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LowCodeImageSaveOptions. Proveedor de opciones de guardado para guardar imágenes generadas"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodeimagesaveoptions/saveoptionsprovider/
---
## LowCodeImageSaveOptions.SaveOptionsProvider property

Proveedor de opciones de guardado para guardar imágenes generadas.

```csharp
public AbstractLowCodeSaveOptionsProvider SaveOptionsProvider { get; set; }
```

### Observaciones

La salida([`OutputFile`](../../lowcodesaveoptions/outputfile/) o [`OutputStream`](../../lowcodesaveoptions/outputstream/)) especificada por esta instancia no tendrá efecto cuando se especifica esta propiedad. En su lugar, la salida de cada imagen generada será especificada por el proveedor.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeImageSaveOptionsPropertySaveOptionsProviderDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Sample Image Data");
            
            // Crear instancia de LowCodeImageSaveOptions
            LowCodeImageSaveOptions saveOptions = new LowCodeImageSaveOptions();
            saveOptions.SaveFormat = SaveFormat.Png;
            saveOptions.ImageOptions = new ImageOrPrintOptions();
            
            // Crear un SaveOptionsProvider personalizado
            CustomSaveOptionsProvider provider = new CustomSaveOptionsProvider();
            saveOptions.SaveOptionsProvider = provider;
            
            // Mostrar SaveOptionsProvider actual
            Console.WriteLine("Current SaveOptionsProvider: " + (saveOptions.SaveOptionsProvider != null ? "Custom Provider" : "null"));
            
            // Demostrar el efecto guardando con diferentes opciones
            workbook.Save("output_with_provider.png", saveOptions.SaveFormat);
            
            // Cambiar a proveedor nulo
            saveOptions.SaveOptionsProvider = null;
            Console.WriteLine("Changed SaveOptionsProvider to: " + (saveOptions.SaveOptionsProvider != null ? "Custom Provider" : "null"));
            
            workbook.Save("output_without_provider.png", saveOptions.SaveFormat);
        }
    }

    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            // Devolver opciones de guardado personalizadas para cada parte
            return new LowCodeImageSaveOptions()
            {
                SaveFormat = SaveFormat.Jpg,  // Changed from Jpeg to Jpg
                ImageOptions = new ImageOrPrintOptions()
                {
                    Quality = 90,
                    HorizontalResolution = 300,
                    VerticalResolution = 300
                }
            };
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            // Realizar cualquier limpieza después de guardar
            Console.WriteLine("Finished saving part with custom options");
        }
    }
}
```

### Ver también

* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [LowCodeImageSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


