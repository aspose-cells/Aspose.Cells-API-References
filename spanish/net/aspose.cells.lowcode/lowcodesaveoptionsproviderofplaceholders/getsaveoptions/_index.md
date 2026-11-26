---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.GetSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método LowCodeSaveOptionsProviderOfPlaceHolders. Obtiene las opciones de guardado de las que se extraen los ajustes de salida para la parte dividida actual"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/getsaveoptions/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.GetSaveOptions method

Obtiene las opciones de guardado de las que se extraen los ajustes de salida para la parte dividida actual.

```csharp
public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersMethodGetSaveOptionsWithSplitPartInfoDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear una instancia de SplitPartInfo
            // Dado que SplitPartInfo no tiene un constructor sin parámetros y sus propiedades son de solo lectura,
            // Necesitaremos obtener una instancia desde otro lugar de la API o usar null si está permitido
            // Para fines de demostración, pasaremos null (asumiendo que el método lo acepta)
            SplitPartInfo splitPartInfo = null;

            // Crear la instancia de LowCodeSaveOptionsProviderOfPlaceHolders
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("output_{sheet}.xlsx")
            {
                SheetIndexOffset = 0,
                SplitPartIndexOffset = 0,
                BuildPathWithSheetAlways = false,
                BuildPathWithSplitPartAlways = false,
                SheetNamePrefix = "sheet_",
                SheetIndexPrefix = "sheet_",
                SplitPartPrefix = "part_",
                SaveOptionsTemplate = new LowCodeSaveOptions
                {
                    SaveFormat = SaveFormat.Xlsx
                }
            };

            try
            {
                // Llama al método GetSaveOptions con el parámetro SplitPartInfo
                var saveOptions = provider.GetSaveOptions(splitPartInfo);
                
                Console.WriteLine("GetSaveOptions method executed successfully with SplitPartInfo parameter");
                Console.WriteLine($"Output file: {saveOptions.OutputFile}");
                Console.WriteLine($"Save format: {saveOptions.SaveFormat}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetSaveOptions method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("MethodGetSaveOptionsWithSplitPartInfoDemo.xlsx");
        }
    }
}
```

### Ver también

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SplitPartInfo](../../splitpartinfo/)
* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


