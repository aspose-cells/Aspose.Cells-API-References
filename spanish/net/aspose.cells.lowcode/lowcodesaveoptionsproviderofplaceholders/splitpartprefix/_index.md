---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SplitPartPrefix"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LowCodeSaveOptionsProviderOfPlaceHolders. Prefijo para el índice de la parte dividida"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartprefix/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SplitPartPrefix property

Prefijo para el índice de la parte dividida.

```csharp
public string SplitPartPrefix { get; set; }
```

### Observaciones

Si solo hay una parte dividida y [`BuildPathWithSplitPartAlways`](../buildpathwithsplitpartalways/) es false, entonces este prefijo y el índice de la parte dividida (0) no se agregarán a la ruta del archivo resultante.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySplitPartPrefixDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            for (int i = 0; i < 25; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data row {i + 1}";
            }

            // Configurar plantilla de opciones de guardado
            LowCodeSaveOptions saveOptionsTemplate = new LowCodeSaveOptions();

            // Inicializar el proveedor con el marcador de posición de la parte dividida
            LowCodeSaveOptionsProviderOfPlaceHolders provider = new LowCodeSaveOptionsProviderOfPlaceHolders("SplitResult_Sheet{sheet}_Part{split}.xlsx")
            {
                SaveOptionsTemplate = saveOptionsTemplate
            };

            // Mostrar y modificar SplitPartPrefix
            Console.WriteLine($"Initial SplitPartPrefix: {provider.SplitPartPrefix}");
            provider.SplitPartPrefix = "Section";
            Console.WriteLine($"Updated SplitPartPrefix: {provider.SplitPartPrefix}");

            // Guardar el libro de trabajo con partes divididas usando el formato de guardado del proveedor
            workbook.Save("output", saveOptionsTemplate.SaveFormat);

            Console.WriteLine("Check 'output' directory for split files with 'Section' prefix");
        }
    }
}
```

### Ver también

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


