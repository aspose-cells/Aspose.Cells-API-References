---
title: "Klass MarkdownSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.MarkdownSaveOptions‑klass. Representerar sparalternativen för markdown"
type: docs
url: /sv/net/aspose.cells/markdownsaveoptions/
---
## MarkdownSaveOptions class

Representerar sparalternativen för markdown.

```csharp
public class MarkdownSaveOptions : SaveOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [MarkdownSaveOptions](markdownsaveoptions/)() | Skapar alternativ för att spara markdown‑dokument |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AlignColumnPadding](../../aspose.cells/markdownsaveoptions/aligncolumnpadding/) { get; set; } | Anger om kolumnjustering är aktiverad för genererade Markdown‑tabeller. När den är aktiverad justeras kolumnerna genom att fylla cellinnehållet med det angivna tecknet (vanligtvis ' ' för mellanslag). Ställ in på '\\0' för att inaktivera kolumnjustering (standard). |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Mappen för temporära filer som kan användas som datacache. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CalculateFormula](../../aspose.cells/markdownsaveoptions/calculateformula/) { get; set; } | Anger om formler ska beräknas innan markdown‑filen sparas. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Om restriktioner för Excel‑filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32 K. När du matar in ett värde längre än 32 K kommer det att trunkeras. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Gör arbetsboken tom efter att filen har sparats. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [Encoding](../../aspose.cells/markdownsaveoptions/encoding/) { get; set; } | Hämtar och anger standardkodningen. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Anger om dokumentegenskaper ska krypteras när du sparar som .xls‑fil. Standardvärdet är true. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ExportHyperlinkAsReference](../../aspose.cells/markdownsaveoptions/exporthyperlinkasreference/) { get; set; } | Anger om hyperlänken ska exporteras med referensdefinitioner istället för inline-format. Standardvärdet är falskt. |
| [ExportImagesAsBase64](../../aspose.cells/markdownsaveoptions/exportimagesasbase64/) { get; set; } | Anger om bilder sparas i Base64-format till Markdown. Standardvärdet är sant. |
| [FormatStrategy](../../aspose.cells/markdownsaveoptions/formatstrategy/) { get; set; } | Hämtar och anger formatstrategin när cellvärdet exporteras som sträng. |
| [ImageOptions](../../aspose.cells/markdownsaveoptions/imageoptions/) { get; } | Hämta ImageOrPrintOptions-objektet innan export |
| [LightCellsDataProvider](../../aspose.cells/markdownsaveoptions/lightcellsdataprovider/) { get; set; } | Dataleverantören som tillhandahåller celldata för att spara arbetsboken i lättläge. |
| [LineSeparator](../../aspose.cells/markdownsaveoptions/lineseparator/) { get; set; } | Hämtar och anger radseparatorn. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [OfficeMathOutputType](../../aspose.cells/markdownsaveoptions/officemathoutputtype/) { get; set; } | Anger hur OfficeMath-objekt exporteras till Markdown. Standardvärdet är Image. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Anger om den senaste diagramdata ska cachas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Hämtar sparfilformatet. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SheetSet](../../aspose.cells/markdownsaveoptions/sheetset/) { get; set; } | Hämtar eller anger bladen som ska renderas. Standard är alla synliga blad i arbetsboken: [`Active`](../../aspose.cells.rendering/sheetset/active/). |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Anger om externa definierade namn ska sorteras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Anger om definierade namn ska sorteras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SplitTablesByBlankRow](../../aspose.cells/markdownsaveoptions/splittablesbyblankrow/) { get; set; } | Anger om tomma rader i arbetsbladet ska behandlas som tabellseparatorer vid export till Markdown. Standardvärdet är falskt. |
| [StreamProvider](../../aspose.cells/markdownsaveoptions/streamprovider/) { get; set; } | Hämtar eller anger IStreamProvider för export av objekt. Om `null` sparas de exporterade objekten i samma katalog som utdatafilen. |
| [TableHeaderType](../../aspose.cells/markdownsaveoptions/tableheadertype/) { get; set; } | Hämtar och anger hur tabellens rubrik ska sättas. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Anger om inställning för smart art ska uppdateras. Standardvärdet är false. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Anger om sammanslagna celler ska valideras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Hämtar eller anger varningsåteranrop.(Ärvd från [`SaveOptions`](../saveoptions/).) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Text;

    public class MarkdownSaveOptionsDemo
    {
        public static void MarkdownSaveOptionsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i kalkylbladet
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Skapa en instans av MarkdownSaveOptions
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
            {
                Encoding = Encoding.UTF8,
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                LineSeparator = "\n",
                ClearData = false,
                CachedFileFolder = "C:\\Temp",
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = false,
                SortExternalNames = false,
                RefreshChartCache = false,
                UpdateSmartArt = false
            };

            // Spara arbetsboken som en Markdown-fil
            workbook.Save("MarkdownSaveOptionsExample.md", saveOptions);

            Console.WriteLine("Workbook saved as Markdown file successfully.");
        }
    }
}
```

### Se även

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


