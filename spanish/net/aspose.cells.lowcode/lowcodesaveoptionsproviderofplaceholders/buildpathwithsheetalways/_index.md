---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSheetAlways"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LowCodeSaveOptionsProviderOfPlaceHolders. Indica si se agrega siempre el índice o nombre de la hoja a la ruta del archivo. El valor predeterminado es false, lo que significa que cuando solo hay una hoja, el índice y nombre de la hoja y el prefijo correspondiente prefixSheetNamePrefix no se agregarán a la ruta del archivo."
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsheetalways/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSheetAlways property

Indica si se agrega siempre el índice o nombre de la hoja a la ruta del archivo. El valor predeterminado es false, es decir, cuando solo hay una hoja, el índice y nombre de la hoja y el prefijo correspondiente ([`SheetNamePrefix`](../sheetnameprefix/)) no se agregarán a la ruta del archivo.

```csharp
public bool BuildPathWithSheetAlways { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertyBuildPathWithSheetAlwaysDemo
    {
        public static void Run()
        {
            // Crear libro de trabajo con dos hojas para demostrar diferencias de ruta
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Configurar proveedor con marcador de posición de índice de hoja
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("Output_{sheet_index}.xlsx")
            {
                // Demostrar desplazamiento del índice de hoja (opcional)
                SheetIndexOffset = 1
            };

            Console.WriteLine($"Initial BuildPathWithSheetAlways: {provider.BuildPathWithSheetAlways}");

            // Guardar con índice de hoja solo cuando hay múltiples hojas (comportamiento predeterminado)
            provider.BuildPathWithSheetAlways = false;
            SaveWithProvider(workbook, provider, "DefaultBehavior");

            // Forzar índice de hoja en los nombres de archivo incluso para hojas únicas
            provider.BuildPathWithSheetAlways = true;
            Console.WriteLine($"Modified BuildPathWithSheetAlways: {provider.BuildPathWithSheetAlways}");
            SaveWithProvider(workbook, provider, "ForcedSheetIndex");
        }

        private static void SaveWithProvider(Workbook workbook, LowCodeSaveOptionsProviderOfPlaceHolders provider, string saveDescription)
        {
            // Configurar opciones de guardado con formato JSON para habilitar la división
            var saveOptions = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Json
            };

            // Configurar el proveedor con las opciones de guardado
            provider.SaveOptionsTemplate = saveOptions;

            // Guardar con rutas determinadas por el proveedor
            Console.WriteLine($"Saving with {saveDescription} - check output files");
            workbook.Save($"dummy_{saveDescription}.json", saveOptions.SaveFormat);
        }
    }
}
```

### Ver también

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


