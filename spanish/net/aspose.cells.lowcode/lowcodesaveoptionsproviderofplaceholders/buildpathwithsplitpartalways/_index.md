---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSplitPartAlways"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LowCodeSaveOptionsProviderOfPlaceHolders. Indica si se agrega siempre el índice de la parte dividida a la ruta del archivo. El valor predeterminado es false, lo que significa que cuando solo hay una parte dividida, el índice de la parte dividida y el prefijo correspondiente prefixSplitPartPrefix no se agregarán a la ruta del archivo."
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsplitpartalways/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSplitPartAlways property

Indica si se agrega siempre el índice de la parte dividida a la ruta del archivo. El valor predeterminado es false, es decir, cuando solo hay una parte dividida, el índice de la parte dividida y el prefijo correspondiente ([`SplitPartPrefix`](../splitpartprefix/)) no se agregarán a la ruta del archivo.

```csharp
public bool BuildPathWithSplitPartAlways { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertyBuildPathWithSplitPartAlwaysDemo
    {
        public static void Run()
        {
            // Crear libro de trabajo con datos que no se dividirán en múltiples partes
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Single Part Demonstration";

            // Crear proveedor con plantilla de ruta y condición de división que resulte en una sola parte
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("Result_{split}.xlsx")
            {
                SaveOptionsTemplate = new LowCodeSaveOptions()
            };

            // Demostrar estado false de la propiedad (predeterminado)
            Console.WriteLine($"Initial BuildPathWithSplitPartAlways: {provider.BuildPathWithSplitPartAlways}");
            provider.BuildPathWithSplitPartAlways = false;
            
            // Esto generaría Result.xlsx cuando solo existe una parte
            Console.WriteLine("Saving with BuildPathWithSplitPartAlways=false");
            ExecuteDummySave(workbook, "Result.xlsx");

            // Alternar la propiedad y demostrar el estado true
            provider.BuildPathWithSplitPartAlways = true;
            Console.WriteLine("\nSaving with BuildPathWithSplitPartAlways=true");
            
            // Esto generaría Result_0.xlsx incluso con una sola parte
            ExecuteDummySave(workbook, "Result_0.xlsx");
        }

        private static void ExecuteDummySave(Workbook workbook, string filename)
        {
            // En uso real, reemplazar con la operación de guardado basada en proveedor
            Console.WriteLine($"Simulated save operation -> Filename: {filename}");
            workbook.Save(filename, SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


