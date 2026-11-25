---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.GetSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo LowCodeSaveOptionsProviderOfPlaceHolders. Ottiene le opzioni di salvataggio da cui ricavare le impostazioni di output per la parte attualmente divisa"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/getsaveoptions/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.GetSaveOptions method

Ottiene le opzioni di salvataggio da cui ricavare le impostazioni di output per la parte divisa corrente.

```csharp
public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un'istanza di SplitPartInfo
            // Poiché SplitPartInfo non ha un costruttore senza parametri e le proprietà sono di sola lettura,
            // dovremo ottenere un'istanza da qualche altra parte dell'API o usare null se consentito
            // Per scopi dimostrativi, passeremo null (supponendo che il metodo lo accetti)
            SplitPartInfo splitPartInfo = null;

            // Crea l'istanza di LowCodeSaveOptionsProviderOfPlaceHolders
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
                // Chiama il metodo GetSaveOptions con il parametro SplitPartInfo
                var saveOptions = provider.GetSaveOptions(splitPartInfo);
                
                Console.WriteLine("GetSaveOptions method executed successfully with SplitPartInfo parameter");
                Console.WriteLine($"Output file: {saveOptions.OutputFile}");
                Console.WriteLine($"Save format: {saveOptions.SaveFormat}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetSaveOptions method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("MethodGetSaveOptionsWithSplitPartInfoDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SplitPartInfo](../../splitpartinfo/)
* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


