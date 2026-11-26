---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SplitPartIndexOffset"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LowCodeSaveOptionsProviderOfPlaceHolders. Desplazamiento del índice de partes divididas entre lo que se usa en la ruta del archivo y su valor real valuePartIndex"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartindexoffset/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SplitPartIndexOffset property

Desplazamiento del índice de la parte dividida entre lo que se usa en la ruta del archivo y su valor real ([`PartIndex`](../../splitpartinfo/partindex/)).

```csharp
public int SplitPartIndexOffset { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySplitPartIndexOffsetDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 15; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data Row {i + 1}";
            }

            // Crear plantilla de opciones de guardado de bajo código
            LowCodeSaveOptions saveOptionsTemplate = new LowCodeSaveOptions();
            saveOptionsTemplate.SaveFormat = SaveFormat.Xlsx;

            // Inicializar proveedor con plantilla de ruta
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("output/SplitPart_{0}.xlsx");
            provider.SaveOptionsTemplate = saveOptionsTemplate;

            // Mostrar y modificar SplitPartIndexOffset
            Console.WriteLine("Initial SplitPartIndexOffset: " + provider.SplitPartIndexOffset);
            provider.SplitPartIndexOffset = 1;

            // Guardar libro de trabajo para generar partes divididas con índice ajustado
            workbook.Save("SplitPartIndexOffsetDemo", saveOptionsTemplate.SaveFormat);

            Console.WriteLine("Generated split parts with offset applied.");
        }
    }
}
```

### Ver también

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


