---
title: "Klass LowCodeSaveOptionsProviderOfAssembling"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.LowCode.LowCodeSaveOptionsProviderOfAssembling-klass. Implementation för att tillhandahålla sparaalternativ som sparar uppdelade delar till filer och sökvägen för den resulterande filen namnges som det kan innehålla kataloger PathHeaderSheetPrefixSheetIndexor SheetName SplitPartPrefixSplitPartIndexPathTail"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/
---
## LowCodeSaveOptionsProviderOfAssembling class

Implementation för att tillhandahålla sparaalternativ som sparar uppdelade delar till filer och sökvägen för den resulterande filen namnges som (det kan innehålla kataloger): [`PathHeader`](./pathheader/)+[`SheetPrefix`](./sheetprefix/)+SheetIndex(eller SheetName)+[`SplitPartPrefix`](./splitpartprefix/)+SplitPartIndex+[`PathTail`](./pathtail/).

```csharp
public class LowCodeSaveOptionsProviderOfAssembling : AbstractLowCodeSaveOptionsProvider
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [LowCodeSaveOptionsProviderOfAssembling](lowcodesaveoptionsproviderofassembling/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BuildPathWithSheetAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsheetalways/) { get; set; } | Om bladindex eller namn alltid ska läggas till i filsökvägen. Standardvärdet är falskt, det vill säga när det bara finns ett blad, kommer bladindex (eller namn) och motsvarande prefix inte att läggas till i filsökvägen. |
| [BuildPathWithSplitPartAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsplitpartalways/) { get; set; } | Om delningsdelens index alltid ska läggas till i filsökvägen. Standardvärdet är falskt, det vill säga när det bara finns en delningsdel, kommer delningsdelens index och motsvarande prefix inte att läggas till i filsökvägen. |
| [PathHeader](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathheader/) { get; set; } | Headerdel (innan tillagt innehåll från blad och delningsdel) av filsökvägen. |
| [PathTail](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathtail/) { get; set; } | Avslutningsdel (efter sekvensnummer) av filsökvägen. Den bör inkludera filnamnstillägget. |
| [SaveOptionsTemplate](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/saveoptionstemplate/) { get; set; } | Mallen för att skapa en instans av sparaalternativ i [`GetSaveOptions`](./getsaveoptions/). |
| [SheetIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetindexoffset/) { get; set; } | Offset för bladets index mellan vad som används i filsökvägen och dess faktiska värde ([`SheetIndex`](../splitpartinfo/sheetindex/)). |
| [SheetPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetprefix/) { get; set; } | Prefix för indexet för kalkylbladet. |
| [SplitPartIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartindexoffset/) { get; set; } | Offset för delningsdelens index mellan vad som används i filsökvägen och dess faktiska värde ([`PartIndex`](../splitpartinfo/partindex/)). |
| [SplitPartPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartprefix/) { get; set; } | Prefix för indexet för delningsdelen. |
| [UseSheetName](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/usesheetname/) { get; set; } | Om filvägen byggs med bladnamn istället för bladindex. Standardvärdet är falskt. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | Frigör resurser efter bearbetning av den aktuella delade delen.(Ärvd från [`AbstractLowCodeSaveOptionsProvider`](../abstractlowcodesaveoptionsprovider/).) |
| override [GetSaveOptions](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/getsaveoptions/)(SplitPartInfo) | Hämtar sparalternativen som används för att få utdatainställningarna för den aktuella delade delen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Saving;

    public class LowCodeClassLowCodeSaveOptionsProviderOfAssemblingDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data {i + 1}";
            }

            // Initiera och konfigurera sparalternativleverantören
            LowCodeSaveOptionsProviderOfAssembling provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "SplitOutput/",
                PathTail = "_Part.xlsx",
                UseSheetName = true,
                SheetPrefix = "SHEET-",
                SplitPartPrefix = "PART-",
                BuildPathWithSheetAlways = true,
                BuildPathWithSplitPartAlways = true,
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
            };

            // Konfigurera XLSX-sparalternativ med uppdelning med hjälp av LowCodeSaveOptions
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Xlsx
            };

            // Spara arbetsbok med leverantörsaktiverade alternativ med korrekt sparformat
            workbook.Save("LowCodeSaveOptionsProviderOfAssemblingDemo_Output.xlsx", saveOptions.SaveFormat);
        }
    }
}
```

### Se även

* class [AbstractLowCodeSaveOptionsProvider](../abstractlowcodesaveoptionsprovider/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


