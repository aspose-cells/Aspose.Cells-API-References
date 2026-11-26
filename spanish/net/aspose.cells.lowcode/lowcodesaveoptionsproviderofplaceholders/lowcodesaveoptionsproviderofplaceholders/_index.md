---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor de LowCodeSaveOptionsProviderOfPlaceHolders. Instancia un objeto para proporcionar opciones de guardado según plantillas especificadas"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/lowcodesaveoptionsproviderofplaceholders/
---
## LowCodeSaveOptionsProviderOfPlaceHolders constructor

Instancia un objeto para proporcionar opciones de guardado según plantillas especificadas.

```csharp
public LowCodeSaveOptionsProviderOfPlaceHolders(string pathTemplate)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pathTemplate | String | La plantilla de la ruta de archivo resultante. |

### Observaciones

Los marcadores de posición compatibles en la plantilla de ruta de archivo: ${SheetIndex}: será reemplazado por el índice de hoja de la parte dividida${SheetName}: será reemplazado por el nombre de hoja de la parte dividida${SplitPartIndex}: será reemplazado por el índice de la parte dividida${SheetIndexPrefix}: será reemplazado por [`SheetIndexPrefix`](../sheetindexprefix/)${SheetNamePrefix}: será reemplazado por [`SheetNamePrefix`](../sheetnameprefix/)${SplitPartPrefix}: será reemplazado por [`SplitPartPrefix`](../splitpartprefix/)

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersMethodCtorWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Llama al método #ctor con un parámetro String
                string pathTemplate = "output_{sheet}_part_{part}.xlsx";
                var provider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

                // Establecer algunas propiedades
                provider.SheetIndexOffset = 0;
                provider.SplitPartIndexOffset = 0;
                provider.SheetNamePrefix = "Sheet_";
                provider.SplitPartPrefix = "Part_";

                Console.WriteLine("LowCodeSaveOptionsProviderOfPlaceHolders created successfully with path template: " + pathTemplate);
                Console.WriteLine($"SheetNamePrefix: {provider.SheetNamePrefix}, SplitPartPrefix: {provider.SplitPartPrefix}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating LowCodeSaveOptionsProviderOfPlaceHolders: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("LowCodeSaveOptionsProviderDemo.xlsx");
        }
    }
}
```

### Ver también

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


