---
title: "Klass LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.LowCode.LowCodeSaveOptionsProviderOfPlaceHolders-klass. Implementering för att tillhandahålla sparalternativ som sparar delade delar till filer och sökvägen för den resulterande filen definieras med platshållare"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/
---
## LowCodeSaveOptionsProviderOfPlaceHolders class

Implementering för att tillhandahålla sparalternativ som sparar delade delar till filer och sökvägen för den resulterande filen definieras med platshållare.

```csharp
public class LowCodeSaveOptionsProviderOfPlaceHolders : AbstractLowCodeSaveOptionsProvider
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [LowCodeSaveOptionsProviderOfPlaceHolders](lowcodesaveoptionsproviderofplaceholders/)(string) | Instansierar ett objekt för att tillhandahålla sparalternativ enligt angivna mallar. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BuildPathWithSheetAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsheetalways/) { get; set; } | Om bladindex eller namn alltid ska läggas till i filvägen. Standardvärdet är falskt, det vill säga när det bara finns ett blad, kommer bladindex, namn och motsvarande prefix([`SheetNamePrefix`](./sheetnameprefix/)) inte att läggas till i filvägen. |
| [BuildPathWithSplitPartAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsplitpartalways/) { get; set; } | Om delad del-index alltid ska läggas till i filvägen. Standardvärdet är falskt, det vill säga när det bara finns en delad del, kommer del-index och motsvarande prefix([`SplitPartPrefix`](./splitpartprefix/)) inte att läggas till i filvägen. |
| [SaveOptionsTemplate](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/saveoptionstemplate/) { get; set; } | Mallen för att skapa en instans av sparaalternativ i [`GetSaveOptions`](./getsaveoptions/). |
| [SheetIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexoffset/) { get; set; } | Offset för bladets index mellan vad som används i filsökvägen och dess faktiska värde ([`SheetIndex`](../splitpartinfo/sheetindex/)). |
| [SheetIndexPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexprefix/) { get; set; } | Prefix för indexet för kalkylbladet. |
| [SheetNamePrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetnameprefix/) { get; set; } | Prefix för indexet för kalkylbladet. |
| [SplitPartIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartindexoffset/) { get; set; } | Offset för delningsdelens index mellan vad som används i filsökvägen och dess faktiska värde ([`PartIndex`](../splitpartinfo/partindex/)). |
| [SplitPartPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartprefix/) { get; set; } | Prefix för indexet för delningsdelen. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | Frigör resurser efter bearbetning av den aktuella delade delen.(Ärvd från [`AbstractLowCodeSaveOptionsProvider`](../abstractlowcodesaveoptionsprovider/).) |
| override [GetSaveOptions](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/getsaveoptions/)(SplitPartInfo) | Hämtar sparalternativen som används för att få utdatainställningarna för den aktuella delade delen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;

    public class LowCodeClassLowCodeSaveOptionsProviderOfPlaceHoldersDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll i arbetsbladet med exempeldata
            for (int i = 0; i < 250; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data Row {i + 1}";
            }

            // Skapa leverantör med sökvägsmall som innehåller platshållare
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("Output_Sheet_{sheet}_Part_{split}.xlsx");
            
            // Konfigurera leverantörsegenskaper
            provider.SheetIndexOffset = 1;
            provider.SplitPartIndexOffset = 1;
            provider.SheetIndexPrefix = "S";
            provider.SplitPartPrefix = "P";
            provider.BuildPathWithSheetAlways = true;
            provider.BuildPathWithSplitPartAlways = true;

            // Konfigurera mall för sparalternativ
            provider.SaveOptionsTemplate = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Xlsx
            };

            // Konfigurera bild- eller utskriftsalternativ för delad rendering
            var imgOrPrintOptions = new ImageOrPrintOptions
            {
                SaveFormat = SaveFormat.Pdf,
                OnePagePerSheet = false,
                PageIndex = 0,
                PageCount = 1
            };

            // Skapa bladrendering med delad konfiguration
            var sheetRender = new SheetRender(worksheet, imgOrPrintOptions);
            sheetRender.ToImage(0, "output"); // This would normally split and save using provider
        }
    }
}
```

### Se även

* class [AbstractLowCodeSaveOptionsProvider](../abstractlowcodesaveoptionsprovider/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


