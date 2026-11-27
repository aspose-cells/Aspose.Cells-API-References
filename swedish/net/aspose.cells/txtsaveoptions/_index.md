---
title: "Klass TxtSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.TxtSaveOptions-klass. Representerar sparalternativen för csv/tab-avgränsad/annan textformat"
type: docs
url: /sv/net/aspose.cells/txtsaveoptions/
---
## TxtSaveOptions class

Representerar sparalternativen för csv/tab-avgränsad/annan textformat.

```csharp
public class TxtSaveOptions : SaveOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [TxtSaveOptions](txtsaveoptions/#constructor)() | Skapar sparalternativ för textfil. |
| [TxtSaveOptions](txtsaveoptions/#constructor_1)(SaveFormat) | Skapar sparalternativ för textfil. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AlwaysQuoted](../../aspose.cells/txtsaveoptions/alwaysquoted/) { get; set; } | (**Föråldrad.**) Anger om alltid lägga till '\"' för varje fält. Om sant kommer alla värden att omges av citattecken; om falskt kommer värden endast att omges av citattecken när det behövs (till exempel när värden innehåller specialtecken såsom '\"', '\\n' eller separator-tecken). Standard är falskt. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Mappen för temporära filer som kan användas som datacache. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Om restriktioner för Excel‑filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32 K. När du matar in ett värde längre än 32 K kommer det att trunkeras. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Gör arbetsboken tom efter att filen har sparats. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [Encoding](../../aspose.cells/txtsaveoptions/encoding/) { get; set; } | Hämtar och anger standardkodningen. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Anger om dokumentegenskaper ska krypteras när du sparar som .xls‑fil. Standardvärdet är true. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ExportAllSheets](../../aspose.cells/txtsaveoptions/exportallsheets/) { get; set; } | Anger om alla blad ska exporteras till textfilen. Om falskt exporteras endast det aktiva bladet, precis som i MS Excel. |
| [ExportArea](../../aspose.cells/txtsaveoptions/exportarea/) { get; set; } | Intervallet av celler som ska exporteras. |
| [ExportQuotePrefix](../../aspose.cells/txtsaveoptions/exportquoteprefix/) { get; set; } | Anger om enkelfnuttstecknet ska exporteras som en del av värdet i en cell när [`QuotePrefix`](../style/quoteprefix/) är sant för den. Standard är falskt. |
| [FormatStrategy](../../aspose.cells/txtsaveoptions/formatstrategy/) { get; set; } | Hämtar och anger formatstrategin när cellvärdet exporteras som sträng. |
| [KeepSeparatorsForBlankRow](../../aspose.cells/txtsaveoptions/keepseparatorsforblankrow/) { get; set; } | Anger om avgränsare ska skrivas ut för tom rad. Standardvärdet är falskt, så som standard blir innehållet för en tom rad tomt. |
| [LightCellsDataProvider](../../aspose.cells/txtsaveoptions/lightcellsdataprovider/) { get; set; } | Dataleverantören för att spara arbetsboken i lättläge. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [QuoteType](../../aspose.cells/txtsaveoptions/quotetype/) { get; set; } | Hämtar eller anger hur värden ska citeras i den exporterade textfilen. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Anger om den senaste diagramdata ska cachas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Hämtar sparfilformatet. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [Separator](../../aspose.cells/txtsaveoptions/separator/) { get; set; } | Hämtar och anger tecknet avgränsare för textfilen. |
| [SeparatorString](../../aspose.cells/txtsaveoptions/separatorstring/) { get; set; } | Hämtar och anger ett strängvärde som avgränsare. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Anger om externa definierade namn ska sorteras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Anger om definierade namn ska sorteras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [TrimLeadingBlankRowAndColumn](../../aspose.cells/txtsaveoptions/trimleadingblankrowandcolumn/) { get; set; } | Anger om inledande tomma rader och kolumner ska tas bort på samma sätt som i MS Excel. Standard är sant. |
| [TrimTailingBlankCells](../../aspose.cells/txtsaveoptions/trimtailingblankcells/) { get; set; } | Anger om avslutande tomma celler i en rad ska tas bort. Standard är falskt. |
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

    public class TxtSaveOptionsDemo
    {
        public static void TxtSaveOptionsExample()
        {
            // Skapa en arbetsbok med några data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John Doe");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane Smith");
            worksheet.Cells["B3"].PutValue(25);

            // Skapa ett TxtSaveOptions-objekt och ange egenskaper
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Separator = ',',
                SeparatorString = ",",
                Encoding = Encoding.UTF8,
                AlwaysQuoted = false,
                QuoteType = TxtValueQuoteType.Normal,
                FormatStrategy = CellValueFormatStrategy.DisplayStyle,
                TrimLeadingBlankRowAndColumn = true,
                TrimTailingBlankCells = false,
                KeepSeparatorsForBlankRow = false,
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 },
                ExportQuotePrefix = false,
                ExportAllSheets = false,
                ClearData = false,
                CachedFileFolder = "cache",
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = true,
                SortExternalNames = true,
                RefreshChartCache = true,
                UpdateSmartArt = false
            };

            // Spara arbetsboken som en textfil med de angivna alternativen
            workbook.Save("TxtSaveOptionsExample.txt", saveOptions);

            Console.WriteLine("Workbook saved successfully with TxtSaveOptions.");
        }
    }
}
```

### Se även

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


