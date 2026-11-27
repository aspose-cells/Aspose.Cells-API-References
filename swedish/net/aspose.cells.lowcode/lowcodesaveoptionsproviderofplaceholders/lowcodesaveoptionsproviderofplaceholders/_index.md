---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeSaveOptionsProviderOfPlaceHolders‑konstruktor. Skapar en instans för att tillhandahålla sparalternativ enligt angivna mallar"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/lowcodesaveoptionsproviderofplaceholders/
---
## LowCodeSaveOptionsProviderOfPlaceHolders constructor

Instansierar ett objekt för att tillhandahålla sparalternativ enligt angivna mallar.

```csharp
public LowCodeSaveOptionsProviderOfPlaceHolders(string pathTemplate)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pathTemplate | String | Mallen för den resulterande filsökvägen. |

### Anmärkningar

De stödda platshållarna i filsökvägsmallen: ${SheetIndex}: kommer att ersättas med bladindexet för den delade delen${SheetName}: kommer att ersättas med bladnamnet för den delade delen${SplitPartIndex}: kommer att ersättas med indexet för den delade delen${SheetIndexPrefix}: kommer att ersättas med [`SheetIndexPrefix`](../sheetindexprefix/)${SheetNamePrefix}: kommer att ersättas med [`SheetNamePrefix`](../sheetnameprefix/)${SplitPartPrefix}: kommer att ersättas med [`SplitPartPrefix`](../splitpartprefix/)

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Anropa #ctor‑metoden med String‑parameter
                string pathTemplate = "output_{sheet}_part_{part}.xlsx";
                var provider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

                // Ställ in några egenskaper
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

            // Spara arbetsboken
            workbook.Save("LowCodeSaveOptionsProviderDemo.xlsx");
        }
    }
}
```

### Se även

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


