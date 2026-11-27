---
title: "Class XlsSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.XlsSaveOptions class. Representerar sparalternativen för Excel 972003 filformat xls och xlt"
type: docs
url: /sv/net/aspose.cells/xlssaveoptions/
---
## XlsSaveOptions class

Representerar sparalternativen för Excel 97-2003-filformatet: xls och xlt.

```csharp
public class XlsSaveOptions : SaveOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [XlsSaveOptions](xlssaveoptions/#constructor)() | Skapar alternativ för att spara Excel 97‑2003 xls‑fil. |
| [XlsSaveOptions](xlssaveoptions/#constructor_1)(SaveFormat) | Skapar alternativ för att spara Excel 97‑2003 xls/xlt‑fil. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Mappen för temporära filer som kan användas som datacache. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Om restriktioner för Excel‑filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32 K. När du matar in ett värde längre än 32 K kommer det att trunkeras. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Gör arbetsboken tom efter att filen har sparats. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Anger om dokumentegenskaper ska krypteras när du sparar som .xls‑fil. Standardvärdet är true. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [IsTemplate](../../aspose.cells/xlssaveoptions/istemplate/) { get; set; } | (**Obsolete.**) Anger om en mallfil sparas. |
| [LightCellsDataProvider](../../aspose.cells/xlssaveoptions/lightcellsdataprovider/) { get; set; } | Dataleverantören för att spara arbetsboken i lättläge. |
| [MatchColor](../../aspose.cells/xlssaveoptions/matchcolor/) { get; set; } | Anger om teckensnittsfärgen ska matchas eftersom det finns 56 färger i den standardfärgpaletten. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Anger om den senaste diagramdata ska cachas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Hämtar sparfilformatet. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Anger om externa definierade namn ska sorteras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Anger om definierade namn ska sorteras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Anger om inställning för smart art ska uppdateras. Standardvärdet är false. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Anger om sammanslagna celler ska valideras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Hämtar eller anger varningsåteranrop.(Ärvd från [`SaveOptions`](../saveoptions/).) |
| [WpsCompatibility](../../aspose.cells/xlssaveoptions/wpscompatibility/) { get; set; } | (**Obsolete.**) Anger om xls ska göras mer kompatibel med WPS. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XlsSaveOptionsDemo
    {
        public static void XlsSaveOptionsExample()
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

            // Skapa en instans av XlsSaveOptions
            XlsSaveOptions saveOptions = new XlsSaveOptions();

            // Ställa in egenskaper
            saveOptions.MatchColor = true;
            saveOptions.ClearData = false;
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = true;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = false;
            saveOptions.RefreshChartCache = true;
            saveOptions.UpdateSmartArt = false;

            // Spara arbetsboken med de angivna sparalternativen
            workbook.Save("XlsSaveOptionsExample.xlsx", saveOptions);

            return;
        }
    }
}
```

### Se även

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


