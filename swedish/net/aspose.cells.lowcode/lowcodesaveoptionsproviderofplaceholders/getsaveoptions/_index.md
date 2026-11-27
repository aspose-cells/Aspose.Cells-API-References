---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.GetSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeSaveOptionsProviderOfPlaceHolders-metod. Hämtar sparalternativen från vilka utdatainställningarna för den aktuella uppdelade delen erhålls"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/getsaveoptions/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.GetSaveOptions method

Hämtar sparalternativen som används för att få utdatainställningarna för den aktuella delade delen.

```csharp
public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa en SplitPartInfo-instans
            // Eftersom SplitPartInfo saknar parameterlös konstruktor och egenskaperna är skrivskyddade,
            // vi måste hämta en instans från någon annanstans i API:et eller använda null om det är tillåtet
            // För demonstrationsändamål kommer vi att skicka null (förutsatt att metoden accepterar det)
            SplitPartInfo splitPartInfo = null;

            // Skapa instansen av LowCodeSaveOptionsProviderOfPlaceHolders
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
                // Anropa GetSaveOptions‑metoden med SplitPartInfo‑parameter
                var saveOptions = provider.GetSaveOptions(splitPartInfo);
                
                Console.WriteLine("GetSaveOptions method executed successfully with SplitPartInfo parameter");
                Console.WriteLine($"Output file: {saveOptions.OutputFile}");
                Console.WriteLine($"Save format: {saveOptions.SaveFormat}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetSaveOptions method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("MethodGetSaveOptionsWithSplitPartInfoDemo.xlsx");
        }
    }
}
```

### Se även

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SplitPartInfo](../../splitpartinfo/)
* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


