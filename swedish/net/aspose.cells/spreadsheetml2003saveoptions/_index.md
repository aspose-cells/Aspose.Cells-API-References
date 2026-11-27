---
title: "Klass SpreadsheetML2003SaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.SpreadsheetML2003SaveOptions‑klass. Representerar alternativen för att spara Excel 2003‑spreadml‑fil"
type: docs
url: /sv/net/aspose.cells/spreadsheetml2003saveoptions/
---
## SpreadsheetML2003SaveOptions class

Representerar alternativen för att spara Excel 2003‑spreadml‑fil.

```csharp
public class SpreadsheetML2003SaveOptions : SaveOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [SpreadsheetML2003SaveOptions](spreadsheetml2003saveoptions/#constructor)() | Skapar alternativen för att spara Excel 2003‑spreadml‑fil. |
| [SpreadsheetML2003SaveOptions](spreadsheetml2003saveoptions/#constructor_1)(SaveFormat) | (**Obsolete.**) Skapar alternativen för att spara Excel 2003‑spreadml‑fil. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Mappen för temporära filer som kan användas som datacache. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Om restriktioner för Excel‑filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32 K. När du matar in ett värde längre än 32 K kommer det att trunkeras. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Gör arbetsboken tom efter att filen har sparats. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Anger om dokumentegenskaper ska krypteras när du sparar som .xls‑fil. Standardvärdet är true. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ExportColumnIndexOfCell](../../aspose.cells/spreadsheetml2003saveoptions/exportcolumnindexofcell/) { get; set; } | Standardvärdet är false, vilket betyder att kolumnindex ignoreras om cellen är intill den föregående cellen. |
| [IsIndentedFormatting](../../aspose.cells/spreadsheetml2003saveoptions/isindentedformatting/) { get; set; } | Gör så att underordnade element indenteras. |
| [LimitAsXls](../../aspose.cells/spreadsheetml2003saveoptions/limitasxls/) { get; set; } | Begränsning för xls, maximalt radindex är 65535 och maximalt kolumnindex är 255. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Anger om den senaste diagramdata ska cachas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Hämtar sparfilformatet. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Anger om externa definierade namn ska sorteras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Anger om definierade namn ska sorteras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Anger om inställning för smart art ska uppdateras. Standardvärdet är false. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Anger om sammanslagna celler ska valideras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Hämtar eller anger varningsåteranrop.(Ärvd från [`SaveOptions`](../saveoptions/).) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SpreadsheetML2003SaveOptionsDemo
    {
        public static void SpreadsheetML2003SaveOptionsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i lite data i kalkylbladet
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["B2"].PutValue(456);

            // Skapa en instans av SpreadsheetML2003SaveOptions
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();

            // Ställ in egenskaper
            saveOptions.IsIndentedFormatting = true;
            saveOptions.LimitAsXls = false;
            saveOptions.ExportColumnIndexOfCell = true;
            saveOptions.ClearData = false;
            saveOptions.CachedFileFolder = @"C:\Temp";
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = true;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = true;
            saveOptions.RefreshChartCache = true;
            saveOptions.UpdateSmartArt = false;

            // Spara arbetsboken med de angivna sparalternativen
            workbook.Save("SpreadsheetML2003Example.xml", saveOptions);

            return;
        }
    }
}
```

### Se även

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


