---
title: "Klass OoxmlSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.OoxmlSaveOptions‑klass. Representerar alternativen för att spara Office Open XML‑fil"
type: docs
url: /sv/net/aspose.cells/ooxmlsaveoptions/
---
## OoxmlSaveOptions class

Representerar alternativen för att spara Office Open XML-fil.

```csharp
public class OoxmlSaveOptions : SaveOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [OoxmlSaveOptions](ooxmlsaveoptions/#constructor)() | Skapar alternativen för att spara Office Open XML‑fil. |
| [OoxmlSaveOptions](ooxmlsaveoptions/#constructor_1)(SaveFormat) | Skapar alternativen för att spara Office Open XML‑fil. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AsFlatOpc](../../aspose.cells/ooxmlsaveoptions/asflatopc/) { get; set; } | Anger om sparas som en platt OPC‑fil som kan genereras av Open XML SDK. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Mappen för temporära filer som kan användas som datacache. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Om restriktioner för Excel‑filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32 K. När du matar in ett värde längre än 32 K kommer det att trunkeras. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Gör arbetsboken tom efter att filen har sparats. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CompressionType](../../aspose.cells/ooxmlsaveoptions/compressiontype/) { get; set; } | Hämtar och anger komprimeringstypen för ooxml‑fil. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [EmbedOoxmlAsOleObject](../../aspose.cells/ooxmlsaveoptions/embedooxmlasoleobject/) { get; set; } | Anger om Ooxml‑filer för OleObject bäddas in som OLE‑objekt. |
| [EnableZip64](../../aspose.cells/ooxmlsaveoptions/enablezip64/) { get; set; } | Använd ZIP64‑tillägg när du skriver zip‑arkiv, vid behov. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Anger om dokumentegenskaper ska krypteras när du sparar som .xls‑fil. Standardvärdet är true. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ExportCellName](../../aspose.cells/ooxmlsaveoptions/exportcellname/) { get; set; } | Anger om cellnamn ska exporteras till Excel2007 .xlsx (.xlsm, .xltx, .xltm)-fil. Om utdatafilen kan nås av SQL Server DTS måste detta värde vara true. Att sätta värdet till false kommer kraftigt öka prestandan och minska filstorleken vid skapande av stora filer. Standardvärdet är true. |
| [LightCellsDataProvider](../../aspose.cells/ooxmlsaveoptions/lightcellsdataprovider/) { get; set; } | Dataleverantören för att spara arbetsboken i lättläge. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Anger om den senaste diagramdata ska cachas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Hämtar sparfilformatet. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Anger om externa definierade namn ska sorteras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Anger om definierade namn ska sorteras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Anger om inställning för smart art ska uppdateras. Standardvärdet är false. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [UpdateZoom](../../aspose.cells/ooxmlsaveoptions/updatezoom/) { get; set; } | Anger om skalningsfaktorn ska uppdateras innan filen sparas om egenskaperna PageSetup.FitToPagesWide och PageSetup.FitToPagesTall styr hur kalkylbladet skalas. |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Anger om sammanslagna celler ska valideras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Hämtar eller anger varningsåteranrop.(Ärvd från [`SaveOptions`](../saveoptions/).) |
| [WpsCompatibility](../../aspose.cells/ooxmlsaveoptions/wpscompatibility/) { get; set; } | (**Obsolete.**) Anger om xls ska göras mer kompatibel med WPS. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlSaveOptionsDemo
    {
        public static void OoxmlSaveOptionsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i lite data i kalkylbladet
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Skapa en instans av OoxmlSaveOptions
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();

            // Ställa in egenskaper
            saveOptions.ExportCellName = true;
            saveOptions.UpdateZoom = true;
            saveOptions.EnableZip64 = false;
            saveOptions.EmbedOoxmlAsOleObject = false;
            saveOptions.CompressionType = OoxmlCompressionType.Level6;
            saveOptions.ClearData = false;
            saveOptions.CachedFileFolder = "C:\\Temp";
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = false;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = false;
            saveOptions.RefreshChartCache = true;
            saveOptions.UpdateSmartArt = false;

            // Spara arbetsboken med de angivna alternativen
            workbook.Save("OoxmlSaveOptionsExample.xlsx", saveOptions);

            return;
        }
    }
}
```

### Se även

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


