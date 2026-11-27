---
title: "Klass JsonSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.JsonSaveOptions-klass. Representerar alternativen för att spara arbetsboken som en JSON-fil"
type: docs
url: /sv/net/aspose.cells/jsonsaveoptions/
---
## JsonSaveOptions class

Representerar alternativen för att spara arbetsboken som en JSON-fil.

```csharp
public class JsonSaveOptions : SaveOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [JsonSaveOptions](jsonsaveoptions/)() | Skapar alternativ för att spara JSON-fil. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AlwaysExportAsJsonObject](../../aspose.cells/jsonsaveoptions/alwaysexportasjsonobject/) { get; set; } | Anger om Excel alltid ska exporteras till JSON som objekt, även om det bara finns ett arbetsblad i filen. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Mappen för temporära filer som kan användas som datacache. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Om restriktioner för Excel‑filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32 K. När du matar in ett värde längre än 32 K kommer det att trunkeras. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Gör arbetsboken tom efter att filen har sparats. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Anger om dokumentegenskaper ska krypteras när du sparar som .xls‑fil. Standardvärdet är true. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ExportArea](../../aspose.cells/jsonsaveoptions/exportarea/) { get; set; } | Hämtar eller anger exportintervallet. |
| [ExportAsString](../../aspose.cells/jsonsaveoptions/exportasstring/) { get; set; } | Exporterar cellernas strängvärde till JSON. |
| [ExportEmptyCells](../../aspose.cells/jsonsaveoptions/exportemptycells/) { get; set; } | Anger om tomma celler ska exporteras som null. |
| [ExportHyperlinkType](../../aspose.cells/jsonsaveoptions/exporthyperlinktype/) { get; set; } | Representerar typen av export av hyperlänk till JSON. |
| [ExportNestedStructure](../../aspose.cells/jsonsaveoptions/exportnestedstructure/) { get; set; } | Exporterad som parent-child hierarki Json-struktur. |
| [ExportStylePool](../../aspose.cells/jsonsaveoptions/exportstylepool/) { get; set; } | Indikerar om stilar ska exporteras kollektivt eller individuellt till varje cell. |
| [HasHeaderRow](../../aspose.cells/jsonsaveoptions/hasheaderrow/) { get; set; } | Anger om intervallet innehåller en rubrikrad. |
| [Indent](../../aspose.cells/jsonsaveoptions/indent/) { get; set; } | Indikerar indraget. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Anger om den senaste diagramdata ska cachas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Hämtar sparfilformatet. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [Schemas](../../aspose.cells/jsonsaveoptions/schemas/) { get; set; } | Det ursprungliga json-schemat för varje kalkylblad. |
| [SheetIndexes](../../aspose.cells/jsonsaveoptions/sheetindexes/) { get; set; } | Representerar indexen för exporterade blad. |
| [SkipEmptyRows](../../aspose.cells/jsonsaveoptions/skipemptyrows/) { get; set; } | Indikerar om tomma rader ska hoppas över. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Anger om externa definierade namn ska sorteras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Anger om definierade namn ska sorteras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ToExcelStruct](../../aspose.cells/jsonsaveoptions/toexcelstruct/) { get; set; } | Indikerar om konvertering till json-struktur för Excel-filen. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Anger om inställning för smart art ska uppdateras. Standardvärdet är false. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Anger om sammanslagna celler ska valideras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Hämtar eller anger varningsåteranrop.(Ärvd från [`SaveOptions`](../saveoptions/).) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Json;
    using System;

    public class JsonSaveOptionsDemo
    {
        public static void JsonSaveOptionsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i lite data i kalkylbladet
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            // Skapa en instans av JsonSaveOptions
            JsonSaveOptions saveOptions = new JsonSaveOptions
            {
                ExportHyperlinkType = JsonExportHyperlinkType.DisplayString,
                SkipEmptyRows = true,
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 },
                HasHeaderRow = true,
                ExportAsString = true,
                Indent = "  ",
                ExportNestedStructure = false,
                ExportEmptyCells = false,
                AlwaysExportAsJsonObject = false,
                ToExcelStruct = false,
                ClearData = false,
                CachedFileFolder = "C:\\Temp",
                ValidateMergedAreas = true,
                MergeAreas = false,
                SortNames = false,
                SortExternalNames = false,
                RefreshChartCache = false,
                UpdateSmartArt = false
            };

            // Spara arbetsboken som en JSON-fil
            workbook.Save("JsonSaveOptionsExample.json", saveOptions);

            return;
        }
    }
}
```

### Se även

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


