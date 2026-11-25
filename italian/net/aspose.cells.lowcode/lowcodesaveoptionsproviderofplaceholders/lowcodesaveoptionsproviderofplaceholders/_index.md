---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore di LowCodeSaveOptionsProviderOfPlaceHolders. Istanzia un'istanza per fornire opzioni di salvataggio secondo i modelli specificati"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/lowcodesaveoptionsproviderofplaceholders/
---
## LowCodeSaveOptionsProviderOfPlaceHolders constructor

Istanzia un'istanza per fornire le opzioni di salvataggio in base ai modelli specificati.

```csharp
public LowCodeSaveOptionsProviderOfPlaceHolders(string pathTemplate)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pathTemplate | String | Il modello del percorso del file risultante. |

### Osservazioni

I segnaposto supportati nel modello di percorso file: ${SheetIndex}: verrà sostituito con l'indice del foglio della parte divisa${SheetName}: verrà sostituito con il nome del foglio della parte divisa${SplitPartIndex}: verrà sostituito con l'indice della parte divisa${SheetIndexPrefix}: verrà sostituito da [`SheetIndexPrefix`](../sheetindexprefix/)${SheetNamePrefix}: verrà sostituito da [`SheetNamePrefix`](../sheetnameprefix/)${SplitPartPrefix}: verrà sostituito da [`SplitPartPrefix`](../splitpartprefix/)

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Chiama il metodo #ctor con parametro String
                string pathTemplate = "output_{sheet}_part_{part}.xlsx";
                var provider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

                // Imposta alcune proprietà
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

            // Salva la cartella di lavoro
            workbook.Save("LowCodeSaveOptionsProviderDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


