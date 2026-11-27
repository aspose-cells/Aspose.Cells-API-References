---
title: "Klass PdfSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.PdfSaveOptions-klass. Representerar alternativen för att spara pdf‑fil"
type: docs
url: /sv/net/aspose.cells/pdfsaveoptions/
---
## PdfSaveOptions class

Representerar alternativen för att spara pdf-fil.

```csharp
public class PdfSaveOptions : PaginatedSaveOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions/)() | Skapar alternativen för att spara pdf‑fil. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells/paginatedsaveoptions/allcolumnsinonepagepersheet/) { get; set; } | Om AllColumnsInOnePagePerSheet är sant, kommer allt kolumninnehåll i ett blad att skrivas ut på endast en sida i resultatet. Bredden på pappersstorleken i pagesetup ignoreras, och de andra inställningarna för pagesetup kommer fortfarande att tillämpas.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [Bookmark](../../aspose.cells/pdfsaveoptions/bookmark/) { get; set; } | Hämtar och anger [`PdfBookmarkEntry`](../../aspose.cells.rendering/pdfbookmarkentry/)‑objektet. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Mappen för temporära filer som kan användas som datacache. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CalculateFormula](../../aspose.cells/pdfsaveoptions/calculateformula/) { get; set; } | Anger om formler ska beräknas innan pdf‑filen sparas. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Om restriktioner för Excel‑filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32 K. När du matar in ett värde längre än 32 K kommer det att trunkeras. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CheckFontCompatibility](../../aspose.cells/paginatedsaveoptions/checkfontcompatibility/) { get; set; } | Anger om teckensnittskompatibilitet ska kontrolleras för varje tecken i texten.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [CheckWorkbookDefaultFont](../../aspose.cells/paginatedsaveoptions/checkworkbookdefaultfont/) { get; set; } | När tecken i Excel är Unicode och inte har korrekt teckensnitt inställt i cellstilen kan de visas som block i pdf, bild. Ställ in detta till true för att försöka använda arbetsbokens standardteckensnitt för att först visa dessa tecken.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Gör arbetsboken tom efter att filen har sparats. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [Compliance](../../aspose.cells/pdfsaveoptions/compliance/) { get; set; } | Hämtar eller anger PDF‑standardernas efterlevnadsnivå för utdata‑dokument. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CreatedTime](../../aspose.cells/pdfsaveoptions/createdtime/) { get; set; } | Hämtar och anger tiden för generering av pdf‑dokumentet. |
| [CustomPropertiesExport](../../aspose.cells/pdfsaveoptions/custompropertiesexport/) { get; set; } | Hämtar och anger ett värde som bestämmer hur [`CustomDocumentPropertyCollection`](../../aspose.cells.properties/customdocumentpropertycollection/) exporteras till PDF‑fil. Standardvärdet är None. |
| [CustomRenderSettings](../../aspose.cells/paginatedsaveoptions/customrendersettings/) { get; set; } | Hämtar eller anger anpassade inställningar under rendering.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DefaultEditLanguage](../../aspose.cells/paginatedsaveoptions/defaulteditlanguage/) { get; set; } | Hämtar eller anger standardspråk för redigering.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DefaultFont](../../aspose.cells/paginatedsaveoptions/defaultfont/) { get; set; } | När tecken i Excel är Unicode och inte har korrekt teckensnitt inställt i cellstilen kan de visas som block i pdf, bild. Ställ in DefaultFont till exempel MingLiu eller MS Gothic för att visa dessa tecken. Om denna egenskap inte är angiven kommer Aspose.Cells att använda systemets standardteckensnitt för att visa dessa Unicode‑tecken.(Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DisplayDocTitle](../../aspose.cells/pdfsaveoptions/displaydoctitle/) { get; set; } | Anger om fönstrets titellist ska visa dokumenttiteln. |
| [DrawObjectEventHandler](../../aspose.cells/paginatedsaveoptions/drawobjecteventhandler/) { get; set; } | Implementerar detta gränssnitt för att få DrawObject och Bound vid rendering.(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [EmbedAttachments](../../aspose.cells/pdfsaveoptions/embedattachments/) { get; set; } | Anger om bilagor för Ole‑objekt ska bäddas in i Excel. |
| [EmbedStandardWindowsFonts](../../aspose.cells/pdfsaveoptions/embedstandardwindowsfonts/) { get; set; } | Sant för att bädda in TrueType‑teckensnitt. Påverkar endast ASCII‑tecken 32‑127. Teckensnitt för teckenkoder över 127 bäddas alltid in. Teckensnitt bäddas alltid in för PDF/A-1a, PDF/A-1b‑standard. Standard är sant. |
| [EmfRenderSetting](../../aspose.cells/paginatedsaveoptions/emfrendersetting/) { get; set; } | Inställning för rendering av Emf-metafil.(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Anger om dokumentegenskaper ska krypteras när du sparar som .xls‑fil. Standardvärdet är true. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ExportDocumentStructure](../../aspose.cells/pdfsaveoptions/exportdocumentstructure/) { get; set; } | Anger om dokumentstrukturen ska exporteras. |
| [FontEncoding](../../aspose.cells/pdfsaveoptions/fontencoding/) { get; set; } | Hämtar eller anger inbäddad teckenkodning i pdf. |
| [GridlineColor](../../aspose.cells/paginatedsaveoptions/gridlinecolor/) { get; set; } | Hämtar eller anger färg på rutnätlinje.(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [GridlineType](../../aspose.cells/paginatedsaveoptions/gridlinetype/) { get; set; } | Hämtar eller anger typ av rutnätlinje.(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [IgnoreError](../../aspose.cells/paginatedsaveoptions/ignoreerror/) { get; set; } | Anger om du behöver dölja felet vid rendering. Felet kan vara ett fel i form, bild, diagramrendering osv.(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [ImageType](../../aspose.cells/pdfsaveoptions/imagetype/) { get; set; } | (**Föråldrad.**) Representerar bildtypen när diagram och form konverteras. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells/paginatedsaveoptions/isfontsubstitutionchargranularity/) { get; set; } | Anger om endast teckensnittet för tecknet ska ersättas när cellens teckensnitt inte är kompatibelt med det.(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [OnePagePerSheet](../../aspose.cells/paginatedsaveoptions/onepagepersheet/) { get; set; } | Om OnePagePerSheet är sant, kommer allt innehåll i ett blad att skrivas ut på endast en sida i resultatet. Pappersstorleken i pagesetup blir ogiltig, men de andra inställningarna i pagesetup gäller fortfarande.(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [OptimizationType](../../aspose.cells/pdfsaveoptions/optimizationtype/) { get; set; } | Hämtar och anger pdf‑optimeringstyp. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells/paginatedsaveoptions/outputblankpagewhennothingtoprint/) { get; set; } | Anger om en tom sida ska skrivas ut när det inte finns något att skriva ut.(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageCount](../../aspose.cells/paginatedsaveoptions/pagecount/) { get; set; } | Hämtar eller anger antalet sidor att spara.(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageIndex](../../aspose.cells/paginatedsaveoptions/pageindex/) { get; set; } | Hämtar eller anger det 0-baserade indexet för den första sidan att spara.(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageSavingCallback](../../aspose.cells/paginatedsaveoptions/pagesavingcallback/) { get; set; } | Styr/Indikerar framsteg för sid sparningsprocessen.(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PdfCompression](../../aspose.cells/pdfsaveoptions/pdfcompression/) { get; set; } | Ange komprimeringsalgoritmen |
| [PrintingPageType](../../aspose.cells/paginatedsaveoptions/printingpagetype/) { get; set; } | Anger vilka sidor som inte kommer att skrivas ut.(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [Producer](../../aspose.cells/pdfsaveoptions/producer/) { get; set; } | Hämtar och anger producenten av det genererade pdf‑dokumentet. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Anger om den senaste diagramdata ska cachas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [RenderingBehavior](../../aspose.cells/paginatedsaveoptions/renderingbehavior/) { get; set; } | Hämtar eller anger de Excel-specifika renderingsbeteenden som ska tillämpas.(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Hämtar sparfilformatet. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SecurityOptions](../../aspose.cells/pdfsaveoptions/securityoptions/) { get; set; } | Ställ in dessa alternativ när säkerhet behövs i xls2pdf‑resultatet. |
| [SheetSet](../../aspose.cells/paginatedsaveoptions/sheetset/) { get; set; } | Hämtar eller anger bladen som ska renderas. Standard är alla synliga blad i arbetsboken: [`Visible`](../../aspose.cells.rendering/sheetset/visible/).(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Anger om externa definierade namn ska sorteras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Anger om definierade namn ska sorteras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [TextCrossType](../../aspose.cells/paginatedsaveoptions/textcrosstype/) { get; set; } | Hämtar eller anger visningstyp för text när textbredden är större än cellbredden.(Arv från [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Anger om inställning för smart art ska uppdateras. Standardvärdet är false. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Anger om sammanslagna celler ska valideras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Hämtar eller anger varningsåteranrop.(Ärvd från [`SaveOptions`](../saveoptions/).) |
| [Watermark](../../aspose.cells/pdfsaveoptions/watermark/) { get; set; } | Hämtar eller anger vattenstämpel för utdata. |
| [ZoomBehavior](../../aspose.cells/pdfsaveoptions/zoombehavior/) { get; set; } | Hämtar eller anger det initiala visningsläget när det genererade PDF-dokumentet öppnas. Standardvärdet är None. |
| [ZoomFactor](../../aspose.cells/pdfsaveoptions/zoomfactor/) { get; set; } | Hämtar eller anger zoomprocenten som används när [`ZoomBehavior`](./zoombehavior/) är ZoomFactor. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [SetImageResample](../../aspose.cells/pdfsaveoptions/setimageresample/)(int, int) | Anger önskad PPI (pixlar per tum) för omprovningsbilder och JPEG-kvalitet. Alla bilder kommer att konverteras till JPEG med den angivna kvalitetsinställningen, och bilder som är större än den angivna PPI (pixlar per tum) kommer att omprovas. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Rendering.PdfSecurity;
    using System;
    using System.Drawing;

    public class PdfSaveOptionsDemo
    {
        public static void PdfSaveOptionsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells PDF Save Options Example");

            // Skapa en instans av PdfSaveOptions
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Ställ in olika egenskaper
            pdfSaveOptions.EmbedStandardWindowsFonts = true;
            pdfSaveOptions.Compliance = PdfCompliance.PdfA1b;
            pdfSaveOptions.CalculateFormula = true;
            pdfSaveOptions.PdfCompression = PdfCompressionCore.Flate;
            pdfSaveOptions.CreatedTime = DateTime.Now;
            pdfSaveOptions.Producer = "Aspose.Cells";
            pdfSaveOptions.OptimizationType = PdfOptimizationType.MinimumSize;
            pdfSaveOptions.CustomPropertiesExport = PdfCustomPropertiesExport.Standard;
            pdfSaveOptions.ExportDocumentStructure = true;
            pdfSaveOptions.DisplayDocTitle = true;
            pdfSaveOptions.FontEncoding = PdfFontEncoding.Identity;
            pdfSaveOptions.EmbedAttachments = true;
            pdfSaveOptions.DefaultFont = "Arial";
            pdfSaveOptions.CheckWorkbookDefaultFont = true;
            pdfSaveOptions.CheckFontCompatibility = true;
            pdfSaveOptions.IsFontSubstitutionCharGranularity = true;
            pdfSaveOptions.OnePagePerSheet = true;
            pdfSaveOptions.AllColumnsInOnePagePerSheet = true;
            pdfSaveOptions.IgnoreError = true;
            pdfSaveOptions.OutputBlankPageWhenNothingToPrint = true;
            pdfSaveOptions.PageIndex = 0;
            pdfSaveOptions.PageCount = 1;
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;
            pdfSaveOptions.GridlineType = GridlineType.Dotted;
            pdfSaveOptions.TextCrossType = TextCrossType.CrossKeep;
            pdfSaveOptions.DefaultEditLanguage = DefaultEditLanguage.English;
            pdfSaveOptions.SheetSet = SheetSet.Visible;
            pdfSaveOptions.ClearData = true;
            pdfSaveOptions.CachedFileFolder = "C:\\Temp";
            pdfSaveOptions.ValidateMergedAreas = true;
            pdfSaveOptions.MergeAreas = true;
            pdfSaveOptions.SortNames = true;
            pdfSaveOptions.SortExternalNames = true;
            pdfSaveOptions.RefreshChartCache = true;

            // Ställ in säkerhetsalternativ
            PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions
            {
                OwnerPassword = "OwnerPassword",
                UserPassword = "UserPassword",
                PrintPermission = true,
                FullQualityPrintPermission = true
            };
            pdfSaveOptions.SecurityOptions = pdfSecurityOptions;

            // Ställ in vattenstämpel
            RenderingFont font = new RenderingFont("Calibri", 68)
            {
                Italic = true,
                Bold = true,
                Color = Color.Blue
            };
            RenderingWatermark watermark = new RenderingWatermark("Watermark", font)
            {
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                Rotation = 30,
                Opacity = 0.6f,
                ScaleToPagePercent = 50
            };
            pdfSaveOptions.Watermark = watermark;

            // Spara arbetsboken som en PDF-fil
            workbook.Save("PdfSaveOptionsExample.pdf", pdfSaveOptions);
        }
    }
}
```

### Se även

* class [PaginatedSaveOptions](../paginatedsaveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


