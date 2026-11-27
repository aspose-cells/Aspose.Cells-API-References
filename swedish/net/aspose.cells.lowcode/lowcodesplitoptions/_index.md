---
title: "Klass LowCodeSplitOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.LowCode.LowCodeSplitOptions-klass. Alternativ för att dela upp kalkylblad"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesplitoptions/
---
## LowCodeSplitOptions class

Alternativ för att dela kalkylblad.

```csharp
public class LowCodeSplitOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [LowCodeSplitOptions](lowcodesplitoptions/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [LoadOptions](../../aspose.cells.lowcode/lowcodesplitoptions/loadoptions/) { get; set; } | Läsalternativ för att läsa in kalkylbladet som ska delas upp. |
| [SaveOptions](../../aspose.cells.lowcode/lowcodesplitoptions/saveoptions/) { get; set; } | Sparaalternativ för att spara de delade delarna. |
| [SaveOptionsProvider](../../aspose.cells.lowcode/lowcodesplitoptions/saveoptionsprovider/) { get; set; } | Leverantör av sparaalternativ för att spara de delade delarna. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassLowCodeSplitOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll i arbetsbladet med exempeldata
            worksheet.Cells["A1"].PutValue("Sample Data for Splitting");
            
            // Skapa en instans av LowCodeSplitOptions
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            
            // Konfigurera LoadOptions (exempel: hantera lösenordsskyddad källa)
            splitOptions.LoadOptions = new LowCodeLoadOptions();
            
            // Konfigurera SaveOptions (exempel: ange standardutdataformat)
            splitOptions.SaveOptions = new LowCodeSaveOptions();
            
            // Implementera anpassad SaveOptions-leverantör för dynamiska utdatainställningar
            splitOptions.SaveOptionsProvider = new CustomSaveOptionsProvider();
            
            // Exempel på integration: Dela arbetsbok i delar med hjälp av konfigurerade alternativ
            // (Anta att en metod som LowCodeEngine.Split(workbook, splitOptions, "outputDir") finns)
            // LowCodeEngine.Split(workbook, splitOptions, "OutputDirectory");
            
            // Spara den ursprungliga arbetsboken för demonstration
            workbook.Save("LowCodeSplitOptionsDemo.xlsx");
        }

        // Anpassad SaveOptionsProvider-implementation
        private class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
        {
            public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
            {
                // Exempel på logik: Växla inställningar baserat på delningsindex
                return new LowCodeSaveOptions();
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


