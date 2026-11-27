---
title: "Klass AbstractLowCodeSaveOptionsProvider"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.LowCode.AbstractLowCodeSaveOptionsProvider-klass. Implementering för att tillhandahålla flera spara‑alternativ för processer som kräver flera utdata. Till exempel kräver SpreadsheetSplitter‑funktionen flera destinationer för att spara de delade filerna"
type: docs
url: /sv/net/aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/
---
## AbstractLowCodeSaveOptionsProvider class

Implementering för att tillhandahålla flera spara‑alternativ för processer som kräver flera utdata. Till exempel, [`SpreadsheetSplitter`](../spreadsheetsplitter/)‑funktionen kräver flera destinationer för att spara de delade filerna.

```csharp
public abstract class AbstractLowCodeSaveOptionsProvider
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | Frigör resurser efter bearbetning av den aktuella delade delen. |
| abstract [GetSaveOptions](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/getsaveoptions/)(SplitPartInfo) | Hämtar sparalternativen från vilka utdatainställningarna för den aktuella delade delen hämtas. Att returnera null betyder att hoppa över den angivna delen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassAbstractLowCodeSaveOptionsProviderDemo
    {
        public static void Run()
        {
            // Skapa en anpassad leverantör genom att ärva från AbstractLowCodeSaveOptionsProvider
            var customProvider = new CustomSaveOptionsProvider();

            // Skapa en arbetsbok och ett kalkylblad
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll i lite data
            worksheet.Cells["A1"].PutValue("Test Data");
            
            // Skapa information om delad del - i verklig användning skulle detta komma från API:et
            // Eftersom vi inte kan konstruera den direkt, skickar vi bara null för demonstration
            SplitPartInfo splitPartInfo = null;
            
            // Hämta sparalternativ från leverantören
            LowCodeSaveOptions saveOptions = customProvider.GetSaveOptions(splitPartInfo);
            
            // Konfigurera sparalternativ (exempel)
            saveOptions.SaveFormat = SaveFormat.Xlsx;
            
            // Demonstrera avslutning av processen
            customProvider.Finish(saveOptions);
            
            // Spara arbetsboken (inte direkt relaterad till leverantören, bara för demo)
            workbook.Save("LowCodeSaveOptionsDemo.xlsx");
        }
    }

    // Anpassad implementation av AbstractLowCodeSaveOptionsProvider
    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            // Skapa och returnera anpassade sparalternativ baserat på delinformation
            return new LowCodeSaveOptions()
            {
                SaveFormat = SaveFormat.Xlsx
                // Tog bort CachedFileFolder eftersom den inte finns i LowCodeSaveOptions
            };
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            // Rensning eller avslutningslogik här
            Console.WriteLine("Save operation completed for part");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


