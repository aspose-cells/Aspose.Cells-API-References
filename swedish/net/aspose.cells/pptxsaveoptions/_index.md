---
title: "Klass PptxSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.PptxSaveOptions-klass. Representerar pptx‑sparalternativen"
type: docs
url: /sv/net/aspose.cells/pptxsaveoptions/
---
## PptxSaveOptions class

Representerar pptx‑sparaalternativen.

```csharp
public class PptxSaveOptions : PaginatedSaveOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [PptxSaveOptions](pptxsaveoptions/#constructor)() | Representerar pptx‑sparaalternativen. |
| [PptxSaveOptions](pptxsaveoptions/#constructor_1)(bool) | Representerar alternativ för att spara .pptx‑filen. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AdjustFontSizeForRowType](../../aspose.cells/pptxsaveoptions/adjustfontsizeforrowtype/) { get; set; } | Representerar vilken typ av linje som behöver justera teckenstorleken om radens höjd är liten. |
| [AllColumnsInOnePagePerSheet](../../aspose.cells/paginatedsaveoptions/allcolumnsinonepagepersheet/) { get; set; } | Om AllColumnsInOnePagePerSheet är sant, kommer allt kolumninnehåll i ett blad att skrivas ut på endast en sida i resultatet. Bredden på pappersstorleken i pagesetup ignoreras, och de andra inställningarna för pagesetup kommer fortfarande att tillämpas.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [AsFlatOpc](../../aspose.cells/pptxsaveoptions/asflatopc/) { get; set; } | Anger om sparning som en platt opc‑fil som kan genereras av Open XML SDK |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Mappen för temporära filer som kan användas som datacache. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Om restriktioner för Excel‑filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32 K. När du matar in ett värde längre än 32 K kommer det att trunkeras. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CheckFontCompatibility](../../aspose.cells/paginatedsaveoptions/checkfontcompatibility/) { get; set; } | Anger om teckensnittskompatibilitet ska kontrolleras för varje tecken i texten.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [CheckWorkbookDefaultFont](../../aspose.cells/paginatedsaveoptions/checkworkbookdefaultfont/) { get; set; } | När tecken i Excel är Unicode och inte har korrekt teckensnitt inställt i cellstilen kan de visas som block i pdf, bild. Ställ in detta till true för att försöka använda arbetsbokens standardteckensnitt för att först visa dessa tecken.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Gör arbetsboken tom efter att filen har sparats. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CustomRenderSettings](../../aspose.cells/paginatedsaveoptions/customrendersettings/) { get; set; } | Hämtar eller anger anpassade inställningar under rendering.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DefaultEditLanguage](../../aspose.cells/paginatedsaveoptions/defaulteditlanguage/) { get; set; } | Hämtar eller anger standardspråk för redigering.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DefaultFont](../../aspose.cells/paginatedsaveoptions/defaultfont/) { get; set; } | När tecken i Excel är Unicode och inte har korrekt teckensnitt inställt i cellstilen kan de visas som block i pdf, bild. Ställ in DefaultFont till exempel MingLiu eller MS Gothic för att visa dessa tecken. Om denna egenskap inte är angiven kommer Aspose.Cells att använda systemets standardteckensnitt för att visa dessa Unicode‑tecken.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DrawObjectEventHandler](../../aspose.cells/paginatedsaveoptions/drawobjecteventhandler/) { get; set; } | Implementerar detta gränssnitt för att få DrawObject och Bound vid rendering.(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [EmbedXlsxAsChartDataSource](../../aspose.cells/pptxsaveoptions/embedxlsxaschartdatasource/) { get; set; } | Anger om en xlsx‑fil ska bäddas in som datakälla för diagrammet. |
| [EmfRenderSetting](../../aspose.cells/paginatedsaveoptions/emfrendersetting/) { get; set; } | Inställning för rendering av Emf-metafil.(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Anger om dokumentegenskaper ska krypteras när du sparar som .xls‑fil. Standardvärdet är true. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ExportViewType](../../aspose.cells/pptxsaveoptions/exportviewtype/) { get; set; } | Hämtar och anger visningstypen vid export till PowerPoint. Standardexporttypen fungerar som utskrift. |
| [GridlineColor](../../aspose.cells/paginatedsaveoptions/gridlinecolor/) { get; set; } | Hämtar eller anger färg på rutnätlinje.(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [GridlineType](../../aspose.cells/paginatedsaveoptions/gridlinetype/) { get; set; } | Hämtar eller anger typ av rutnätlinje.(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [IgnoreError](../../aspose.cells/paginatedsaveoptions/ignoreerror/) { get; set; } | Anger om du behöver dölja felet vid rendering. Felet kan vara ett fel i form, bild, diagramrendering osv.(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [IgnoreHiddenRows](../../aspose.cells/pptxsaveoptions/ignorehiddenrows/) { get; set; } | Indikerar om dolda rader ska ignoreras vid konvertering från Excel till PowerPoint. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells/paginatedsaveoptions/isfontsubstitutionchargranularity/) { get; set; } | Anger om endast teckensnittet för tecknet ska ersättas när cellens teckensnitt inte är kompatibelt med det.(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [OnePagePerSheet](../../aspose.cells/paginatedsaveoptions/onepagepersheet/) { get; set; } | Om OnePagePerSheet är sant, kommer allt innehåll i ett blad att skrivas ut på endast en sida i resultatet. Pappersstorleken i pagesetup blir ogiltig, men de andra inställningarna i pagesetup gäller fortfarande.(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells/paginatedsaveoptions/outputblankpagewhennothingtoprint/) { get; set; } | Anger om en tom sida ska skrivas ut när det inte finns något att skriva ut.(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageCount](../../aspose.cells/paginatedsaveoptions/pagecount/) { get; set; } | Hämtar eller anger antalet sidor att spara.(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageIndex](../../aspose.cells/paginatedsaveoptions/pageindex/) { get; set; } | Hämtar eller anger det 0-baserade indexet för den första sidan att spara.(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageSavingCallback](../../aspose.cells/paginatedsaveoptions/pagesavingcallback/) { get; set; } | Styr/Indikerar framsteg för sid sparningsprocessen.(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PrintingPageType](../../aspose.cells/paginatedsaveoptions/printingpagetype/) { get; set; } | Anger vilka sidor som inte kommer att skrivas ut.(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Anger om den senaste diagramdata ska cachas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [RenderingBehavior](../../aspose.cells/paginatedsaveoptions/renderingbehavior/) { get; set; } | Hämtar eller anger de Excel-specifika renderingsbeteenden som ska tillämpas.(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [SaveAsEditableShapes](../../aspose.cells/pptxsaveoptions/saveaseditableshapes/) { get; set; } | Spara alla ritobjekt som redigerbara former i pptx‑filen, så att du kan redigera dem i PowerPoint. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Hämtar sparfilformatet. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SheetSet](../../aspose.cells/paginatedsaveoptions/sheetset/) { get; set; } | Hämtar eller anger bladen som ska renderas. Standard är alla synliga blad i arbetsboken: [`Visible`](../../aspose.cells.rendering/sheetset/visible/).(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Anger om externa definierade namn ska sorteras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Anger om definierade namn ska sorteras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [TextCrossType](../../aspose.cells/paginatedsaveoptions/textcrosstype/) { get; set; } | Hämtar eller anger visningstyp för text när textbredden är större än cellbredden.(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Anger om inställning för smart art ska uppdateras. Standardvärdet är false. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Anger om sammanslagna celler ska valideras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Hämtar eller anger varningsåteranrop.(Ärvd från [`SaveOptions`](../saveoptions/).) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Slides;
    using Aspose.Cells.Rendering;
    using System;

    public class PptxSaveOptionsDemo
    {
        public static void PptxSaveOptionsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i lite data i kalkylbladet
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Skapa en instans av PptxSaveOptions
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                IgnoreHiddenRows = true,
                AdjustFontSizeForRowType = AdjustFontSizeForRowType.EmptyRows,
                ExportViewType = SlideViewType.Print,
                DefaultFont = "Arial",
                CheckWorkbookDefaultFont = true,
                CheckFontCompatibility = true,
                IsFontSubstitutionCharGranularity = true,
                OnePagePerSheet = true,
                AllColumnsInOnePagePerSheet = true,
                IgnoreError = true,
                OutputBlankPageWhenNothingToPrint = true,
                PageIndex = 0,
                PageCount = 1,
                PrintingPageType = PrintingPageType.IgnoreBlank,
                GridlineType = GridlineType.Dotted,
                TextCrossType = TextCrossType.CrossKeep,
                DefaultEditLanguage = DefaultEditLanguage.English,
                SheetSet = SheetSet.Visible,
                EmfRenderSetting = EmfRenderSetting.EmfOnly,
                ClearData = true,
                CachedFileFolder = "C:\\Temp",
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = true,
                SortExternalNames = true,
                RefreshChartCache = true,
                UpdateSmartArt = true
            };

            // Spara arbetsboken som en PPTX-fil
            workbook.Save("PptxSaveOptionsExample.pptx", saveOptions);
        }
    }
}
```

### Se även

* class [PaginatedSaveOptions](../paginatedsaveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


