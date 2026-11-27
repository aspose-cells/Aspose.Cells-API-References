---
title: "Klass PaginatedSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.PaginatedSaveOptions klass. Representerar alternativen för paginering"
type: docs
url: /sv/net/aspose.cells/paginatedsaveoptions/
---
## PaginatedSaveOptions class

Representerar alternativen för paginering.

```csharp
public abstract class PaginatedSaveOptions : SaveOptions
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells/paginatedsaveoptions/allcolumnsinonepagepersheet/) { get; set; } | Om AllColumnsInOnePagePerSheet är true, kommer allt kolumninnehåll i ett blad att skrivas ut på endast en sida i resultatet. Bredden på pappersstorleken i sidinställningarna kommer att ignoreras, och de andra inställningarna för sidinställningarna kommer fortfarande att tillämpas. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Mappen för temporära filer som kan användas som datacache. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Om restriktioner för Excel‑filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32 K. När du matar in ett värde längre än 32 K kommer det att trunkeras. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CheckFontCompatibility](../../aspose.cells/paginatedsaveoptions/checkfontcompatibility/) { get; set; } | Anger om teckensnittskompatibilitet ska kontrolleras för varje tecken i texten. |
| [CheckWorkbookDefaultFont](../../aspose.cells/paginatedsaveoptions/checkworkbookdefaultfont/) { get; set; } | När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf, bild. Ställ in detta på true för att försöka använda arbetsbokens standardteckensnitt för att först visa dessa tecken. |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Gör arbetsboken tom efter att filen har sparats. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CustomRenderSettings](../../aspose.cells/paginatedsaveoptions/customrendersettings/) { get; set; } | Hämtar eller anger anpassade inställningar under rendering. |
| [DefaultEditLanguage](../../aspose.cells/paginatedsaveoptions/defaulteditlanguage/) { get; set; } | Hämtar eller anger standardspråket för redigering. |
| [DefaultFont](../../aspose.cells/paginatedsaveoptions/defaultfont/) { get; set; } | När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf, bild. Ställ in DefaultFont, till exempel MingLiu eller MS Gothic, för att visa dessa tecken. Om denna egenskap inte är angiven kommer Aspose.Cells att använda systemets standardteckensnitt för att visa dessa Unicode‑tecken. |
| [DrawObjectEventHandler](../../aspose.cells/paginatedsaveoptions/drawobjecteventhandler/) { get; set; } | Implementerar detta gränssnitt för att hämta DrawObject och Bound vid rendering. |
| [EmfRenderSetting](../../aspose.cells/paginatedsaveoptions/emfrendersetting/) { get; set; } | Inställning för rendering av EMF-metafil. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Anger om dokumentegenskaper ska krypteras när du sparar som .xls‑fil. Standardvärdet är true. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [GridlineColor](../../aspose.cells/paginatedsaveoptions/gridlinecolor/) { get; set; } | Hämtar eller anger färg på rutnätslinjer. |
| [GridlineType](../../aspose.cells/paginatedsaveoptions/gridlinetype/) { get; set; } | Hämtar eller anger typ av rutnätslinje. |
| [IgnoreError](../../aspose.cells/paginatedsaveoptions/ignoreerror/) { get; set; } | Anger om du behöver dölja felet vid rendering. Felet kan vara ett fel i form, bild, diagramrendering osv. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells/paginatedsaveoptions/isfontsubstitutionchargranularity/) { get; set; } | Anger om endast teckensnittet för tecknet ska ersättas när cellens teckensnitt inte är kompatibelt. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [OnePagePerSheet](../../aspose.cells/paginatedsaveoptions/onepagepersheet/) { get; set; } | Om OnePagePerSheet är true kommer allt innehåll i ett blad att skrivas ut på endast en sida i resultatet. Pappersstorleken i pagesetup blir ogiltig, men de övriga inställningarna i pagesetup kommer fortfarande att gälla. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells/paginatedsaveoptions/outputblankpagewhennothingtoprint/) { get; set; } | Anger om en tom sida ska skrivas ut när det inte finns något att skriva ut. |
| [PageCount](../../aspose.cells/paginatedsaveoptions/pagecount/) { get; set; } | Hämtar eller anger antalet sidor som ska sparas. |
| [PageIndex](../../aspose.cells/paginatedsaveoptions/pageindex/) { get; set; } | Hämtar eller anger det 0‑baserade indexet för den första sidan som ska sparas. |
| [PageSavingCallback](../../aspose.cells/paginatedsaveoptions/pagesavingcallback/) { get; set; } | Styr/indikera framsteg för sidlagringsprocessen. |
| [PrintingPageType](../../aspose.cells/paginatedsaveoptions/printingpagetype/) { get; set; } | Anger vilka sidor som inte kommer att skrivas ut. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Anger om den senaste diagramdata ska cachas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [RenderingBehavior](../../aspose.cells/paginatedsaveoptions/renderingbehavior/) { get; set; } | Hämtar eller anger de Excel‑specifika renderingsbeteenden som ska tillämpas. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Hämtar sparfilformatet. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SheetSet](../../aspose.cells/paginatedsaveoptions/sheetset/) { get; set; } | Hämtar eller anger de blad som ska renderas. Standard är alla synliga blad i arbetsboken: [`Visible`](../../aspose.cells.rendering/sheetset/visible/). |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Anger om externa definierade namn ska sorteras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Anger om definierade namn ska sorteras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [TextCrossType](../../aspose.cells/paginatedsaveoptions/textcrosstype/) { get; set; } | Hämtar eller anger visningstyp för text när textbredden är större än cellbredden. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Anger om inställning för smart art ska uppdateras. Standardvärdet är false. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Anger om sammanslagna celler ska valideras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Hämtar eller anger varningsåteranrop.(Ärvd från [`SaveOptions`](../saveoptions/).) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PaginatedSaveOptionsDemo
    {
        public static void PaginatedSaveOptionsExample()
        {
            // Öppna en Excel‑fil
            Workbook workbook = new Workbook("PaginatedSaveOptionsExample_original.xlsx");

            // Skapa en instans av PaginatedSaveOptions
            PdfSaveOptions options = new PdfSaveOptions();

            // Ställa in egenskaper
            options.DefaultFont = "Arial";
            options.CheckWorkbookDefaultFont = true;
            options.CheckFontCompatibility = true;
            options.IsFontSubstitutionCharGranularity = true;
            options.OnePagePerSheet = false;
            options.AllColumnsInOnePagePerSheet = false;
            options.IgnoreError = true;
            options.OutputBlankPageWhenNothingToPrint = false;
            options.PageIndex = 3; // Starting page index (0-based index)
            options.PageCount = 2; // Number of pages to be printed
            options.PrintingPageType = PrintingPageType.IgnoreBlank;
            options.GridlineType = GridlineType.Dotted;
            options.TextCrossType = TextCrossType.CrossKeep;
            options.DefaultEditLanguage = DefaultEditLanguage.English;
            options.SheetSet = new SheetSet(new int[] { workbook.Worksheets.ActiveSheetIndex });
            options.ClearData = false;
            options.CachedFileFolder = "C:\\Temp";
            options.ValidateMergedAreas = true;
            options.MergeAreas = true;
            options.SortNames = true;
            options.SortExternalNames = true;
            options.RefreshChartCache = true;
            options.UpdateSmartArt = false;

            // Spara PDF‑filen
            workbook.Save("PaginatedSaveOptionsExample.pdf", options);

            return;
        }
    }
}
```

### Se även

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


