---
title: "Klass HtmlSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.HtmlSaveOptions-klass. Representerar alternativen för att spara en html‑fil."
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/
---
## HtmlSaveOptions class

Representerar alternativen för att spara HTML-fil.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions/#constructor)() | Skapar alternativ för att spara en html‑fil. |
| [HtmlSaveOptions](htmlsaveoptions/#constructor_1)(SaveFormat) | Skapar alternativ för att spara en htm‑fil. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AddGenericFont](../../aspose.cells/htmlsaveoptions/addgenericfont/) { get; set; } | Anger om en generisk teckensnitt ska läggas till i CSS font-family. Standardvärdet är true |
| [AddTooltipText](../../aspose.cells/htmlsaveoptions/addtooltiptext/) { get; set; } | Anger om tooltip‑text ska läggas till när data inte kan visas helt. Standardvärdet är false. |
| [AttachedFilesDirectory](../../aspose.cells/htmlsaveoptions/attachedfilesdirectory/) { get; set; } | Den katalog som de bifogade filerna kommer att sparas i. Endast för att spara till html‑ström. |
| [AttachedFilesUrlPrefix](../../aspose.cells/htmlsaveoptions/attachedfilesurlprefix/) { get; set; } | Ange Url‑prefixet för bifogade filer, såsom bild i html‑filen. Endast för att spara till html‑ström. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Mappen för temporära filer som kan användas som datacache. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CalculateFormula](../../aspose.cells/htmlsaveoptions/calculateformula/) { get; set; } | Anger om formler ska beräknas innan html‑filen sparas. |
| [CellCssPrefix](../../aspose.cells/htmlsaveoptions/cellcssprefix/) { get; set; } | Hämtar och anger prefixet för css‑namnet, standardvärdet är "". |
| [CellNameAttribute](../../aspose.cells/htmlsaveoptions/cellnameattribute/) { get; set; } | Anger attributet som visar CellName som ska skrivas. (t.ex. Om värdet är "id", så blir utskriften för cellen "A1" &lt;td id='A1'&gt;). Standardvärdet är null. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Om restriktioner för Excel‑filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32 K. När du matar in ett värde längre än 32 K kommer det att trunkeras. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Gör arbetsboken tom efter att filen har sparats. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [CssStyles](../../aspose.cells/htmlsaveoptions/cssstyles/) { get; set; } | Hämtar eller anger de extra css‑stilarna för formateraren. Fungerar endast när [`SaveAsSingleFile`](./saveassinglefile/) är True.  CssStyles="body { padding: 5px }"; |
| [DataBarRenderMode](../../aspose.cells/htmlsaveoptions/databarrendermode/) { get; set; } | Representerar läget för hur DataBar renderas när Excel‑filer konverteras till html‑filer. Standardvärdet är BackgroundColor. |
| [DefaultFontName](../../aspose.cells/htmlsaveoptions/defaultfontname/) { get; set; } | Ange standardteckensnittets namn för export av html, standardteckensnittet används när stilens teckensnitt inte finns. Om denna egenskap är null kommer Aspose.Cells att använda ett universellt teckensnitt som har samma familj som originalteckensnittet, standardvärdet är null. |
| [DisableCss](../../aspose.cells/htmlsaveoptions/disablecss/) { get; set; } | Anger om endast inline‑stilar ska tillämpas, utan att förlita sig på CSS. Standardvärdet är false. |
| [DisableDownlevelRevealedComments](../../aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments/) { get; set; } | Anger om Downlevel‑revealed villkorliga kommentarer ska inaktiveras vid export av fil till html, standardvärdet är false. |
| [EmbeddedFontType](../../aspose.cells/htmlsaveoptions/embeddedfonttype/) { get; set; } | Hämtar eller anger typen av inbäddning av teckensnittsfiler i html‑filen. Standardvärdet är None vilket indikerar att inget teckensnitt kommer att bäddas in i html. |
| [EnableCssCustomProperties](../../aspose.cells/htmlsaveoptions/enablecsscustomproperties/) { get; set; } | Optimera html‑utdata genom att använda CSS‑anpassade egenskaper. Till exempel, i scenariot där en base64‑bild förekommer flera gånger, krävs bilddata endast sparas en gång med en anpassad egenskap, vilket kan förbättra prestandan för den resulterande html‑filen. Standardvärdet är false. |
| [EncodeEntityAsCode](../../aspose.cells/htmlsaveoptions/encodeentityascode/) { get; set; } | Anger om html‑teckenentiteter ska ersättas med decimalkod. (t.ex. "&amp;nbsp;" ersätts med "&amp;#160;"). Standardvärdet är false. |
| [Encoding](../../aspose.cells/htmlsaveoptions/encoding/) { get; set; } | Om inte angivet, använd Encoding.UTF8 som standardkodningstyp. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Anger om dokumentegenskaper ska krypteras när du sparar som .xls‑fil. Standardvärdet är true. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ExcludeUnusedStyles](../../aspose.cells/htmlsaveoptions/excludeunusedstyles/) { get; set; } | Anger om oanvända stilar ska uteslutas. För de genererade html‑filerna kan uteslutning av oanvända stilar göra filstorleken mindre utan att påverka den visuella effekten. Så standardvärdet för denna egenskap är true. Om användaren behöver behålla alla stilar i arbetsboken för den genererade html‑filen (t.ex. i scenariot där arbetsboken ska återställas från den genererade html‑filen senare), sätt denna egenskap till false. |
| [ExportActiveWorksheetOnly](../../aspose.cells/htmlsaveoptions/exportactiveworksheetonly/) { get; set; } | Anger om endast det aktiva kalkylbladet ska exporteras till html‑fil. Om true exporteras endast det aktiva kalkylbladet till html‑fil; om false exporteras hela arbetsboken till html‑fil. Standardvärdet är false |
| [ExportArea](../../aspose.cells/htmlsaveoptions/exportarea/) { get; set; } | Hämtar eller anger det exporterade CellArea för det aktuella aktiva kalkylbladet. Om du anger detta attribut kommer utskriftsområdet för det aktuella aktiva kalkylbladet att utelämnas. Endast det angivna området kommer att exporteras när filen sparas som html. |
| [ExportBogusRowData](../../aspose.cells/htmlsaveoptions/exportbogusrowdata/) { get; set; } | Anger om falska data i den nedre raden ska exporteras. Standardvärdet är true. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet. |
| [ExportCellCoordinate](../../aspose.cells/htmlsaveoptions/exportcellcoordinate/) { get; set; } | Anger om Excel-koordinater för icke-tomma celler ska exporteras när filen sparas som html. Standardvärdet är false. Om du vill importera den exporterade html-filen till Excel, behåll standardvärdet. |
| [ExportCommentsType](../../aspose.cells/htmlsaveoptions/exportcommentstype/) { get; set; } | Representerar typ av export av kommentarer till html-filer. |
| [ExportDataOptions](../../aspose.cells/htmlsaveoptions/exportdataoptions/) { get; set; } | Anger regeln för export av html-fildata. Standardvärdet är All. |
| [ExportDocumentProperties](../../aspose.cells/htmlsaveoptions/exportdocumentproperties/) { get; set; } | Anger om dokumentegenskaper ska exporteras. Standardvärdet är true. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet. |
| [ExportExtraHeadings](../../aspose.cells/htmlsaveoptions/exportextraheadings/) { get; set; } | Anger om extra rubriker ska exporteras när textlängden är längre än den maximala visningskolumnen. Standardvärdet är false. Om du vill importera html-filen till Excel, behåll standardvärdet. |
| [ExportFormula](../../aspose.cells/htmlsaveoptions/exportformula/) { get; set; } | Anger om formler ska exporteras när filen sparas som html. Standardvärdet är true. Om du vill importera den exporterade html-filen till Excel, behåll standardvärdet. |
| [ExportFrameScriptsAndProperties](../../aspose.cells/htmlsaveoptions/exportframescriptsandproperties/) { get; set; } | Anger om ram-skript och dokumentegenskaper ska exporteras. Standardvärdet är true. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet. |
| [ExportGridLines](../../aspose.cells/htmlsaveoptions/exportgridlines/) { get; set; } | Anger om rutnät ska exporteras. Standardvärdet är false. |
| [ExportHeadings](../../aspose.cells/htmlsaveoptions/exportheadings/) { get; set; } | (**Obsolete.**) Anger om bladets rad- och kolumnrubriker ska exporteras när man sparar till HTML-filer. |
| [ExportHiddenWorksheet](../../aspose.cells/htmlsaveoptions/exporthiddenworksheet/) { get; set; } | Anger om dolt kalkylbladsinnehåll ska exporteras. Standardvärdet är true. |
| [ExportImagesAsBase64](../../aspose.cells/htmlsaveoptions/exportimagesasbase64/) { get; set; } | Anger om bilder sparas i Base64-format till HTML, MHTML eller EPUB. |
| [ExportNamedRangeAnchors](../../aspose.cells/htmlsaveoptions/exportnamedrangeanchors/) { get; set; } | Anger om ankarelement för namngivna områden ska exporteras när man sparar som HTML. Standardvärdet är true. |
| [ExportObjectListener](../../aspose.cells/htmlsaveoptions/exportobjectlistener/) { get; set; } | (**Obsolete.**) Hämtar eller anger ExportObjectListener för export av objekt. |
| [ExportPageFooters](../../aspose.cells/htmlsaveoptions/exportpagefooters/) { get; set; } | Anger om sidhuvuden ska exporteras. |
| [ExportPageHeaders](../../aspose.cells/htmlsaveoptions/exportpageheaders/) { get; set; } | Anger om sidhuvuden ska exporteras. |
| [ExportPrintAreaOnly](../../aspose.cells/htmlsaveoptions/exportprintareaonly/) { get; set; } | Anger om endast utskriftsområdet ska exporteras till html-fil. Standardvärdet är false. |
| [ExportRowColumnHeadings](../../aspose.cells/htmlsaveoptions/exportrowcolumnheadings/) { get; set; } | Anger om bladets rad- och kolumnrubriker ska exporteras när man sparar till HTML-filer. |
| [ExportSimilarBorderStyle](../../aspose.cells/htmlsaveoptions/exportsimilarborderstyle/) { get; set; } | Anger om liknande ramstil ska exporteras när ramstilen inte stöds av webbläsare. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet. Standardvärdet är false. |
| [ExportSingleTab](../../aspose.cells/htmlsaveoptions/exportsingletab/) { get; set; } | Anger om den enda fliken ska exporteras när filen bara har ett kalkylblad. Standardvärdet är false. |
| [ExportWorkbookProperties](../../aspose.cells/htmlsaveoptions/exportworkbookproperties/) { get; set; } | Anger om arbetsboks egenskaper ska exporteras. Standardvärdet är true. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet. |
| [ExportWorksheetCSSSeparately](../../aspose.cells/htmlsaveoptions/exportworksheetcssseparately/) { get; set; } | Anger om kalkylbladets CSS ska exporteras separat. Standardvärdet är false. |
| [ExportWorksheetProperties](../../aspose.cells/htmlsaveoptions/exportworksheetproperties/) { get; set; } | Anger om kalkylblads egenskaper ska exporteras. Standardvärdet är true. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet. |
| [FilePathProvider](../../aspose.cells/htmlsaveoptions/filepathprovider/) { get; set; } | Hämtar eller anger IFilePathProvider för separat export av kalkylblad till html. |
| [FormatDataIgnoreColumnWidth](../../aspose.cells/htmlsaveoptions/formatdataignorecolumnwidth/) { get; set; } | Anger om hela den formaterade celldata ska visas när den överskrider kolumnen. Om true ignoreras kolumnbredden och hela cellens data exporteras. Om false exporteras data på samma sätt som i Excel. Standardvärdet är false. |
| [HiddenColDisplayType](../../aspose.cells/htmlsaveoptions/hiddencoldisplaytype/) { get; set; } | Dold kolumn (bredden på den här kolumnen är 0) i Excel, innan du sparar detta i HTML-format, om HtmlHiddenColDisplayType är "Remove" kommer den dolda kolumnen inte att skrivas ut, om värdet är "Hidden" kommer kolumnen att skrivas ut men vara dold, standardvärdet är "Hidden" |
| [HiddenRowDisplayType](../../aspose.cells/htmlsaveoptions/hiddenrowdisplaytype/) { get; set; } | Dold rad (höjden på den här raden är 0) i Excel, innan du sparar detta i HTML-format, om HtmlHiddenRowDisplayType är "Remove" kommer den dolda raden inte att skrivas ut, om värdet är "Hidden" kommer raden att skrivas ut men vara dold, standardvärdet är "Hidden" |
| [HideOverflowWrappedText](../../aspose.cells/htmlsaveoptions/hideoverflowwrappedtext/) { get; set; } | Anger om överskjutande text ska döljas när cellformatet är inställt på radbrytning. Standardvärdet är false |
| [HtmlCrossStringType](../../aspose.cells/htmlsaveoptions/htmlcrossstringtype/) { get; set; } | Anger om en sträng som sträcker sig över flera celler ska visas på samma sätt som i MS Excel när en Excel-fil sparas i HTML-format. Som standard är värdet Default, så för strängar som sträcker sig över celler är skillnaden mellan HTML-filerna som skapas av Aspose.Cells och MS Excel liten. Men prestandan för att skapa stora HTML-filer blir flera gånger snabbare om värdet sätts till Cross jämfört med Default eller Fit2Cell. |
| [HtmlVersion](../../aspose.cells/htmlsaveoptions/htmlversion/) { get; set; } | Anger vilken version av HTML-standarden som ska användas när HTML-formatet sparas. Standardvärdet är HtmlVersion.Default. |
| [IgnoreInvisibleShapes](../../aspose.cells/htmlsaveoptions/ignoreinvisibleshapes/) { get; set; } | Anger om osynliga former ska exporteras |
| [ImageOptions](../../aspose.cells/htmlsaveoptions/imageoptions/) { get; } | Hämta ImageOrPrintOptions-objektet innan export |
| [ImageScalable](../../aspose.cells/htmlsaveoptions/imagescalable/) { get; set; } | Anger om en skalbar enhet ska användas för att beskriva bildens bredd när en skalbar enhet används för att beskriva kolumnens bredd. Standardvärdet är true. |
| [IsBorderCollapsed](../../aspose.cells/htmlsaveoptions/isbordercollapsed/) { get; set; } | Anger om tabellramarna är sammanslagna. Standardvärdet är true. |
| [IsExpImageToTempDir](../../aspose.cells/htmlsaveoptions/isexpimagetotempdir/) { get; set; } | Anger om bildfiler ska exporteras till en temporär katalog. Endast för att spara till HTML-ström. |
| [IsExportComments](../../aspose.cells/htmlsaveoptions/isexportcomments/) { get; set; } | Anger om kommentarer ska exporteras när filen sparas i HTML, standardvärdet är false. |
| [IsFullPathLink](../../aspose.cells/htmlsaveoptions/isfullpathlink/) { get; set; } | Anger om fullständig sökväg ska användas i länkar i sheet00x.htm, filelist.xml och tabstrip.htm. Standardvärdet är false. |
| [IsIECompatible](../../aspose.cells/htmlsaveoptions/isiecompatible/) { get; set; } | Anger om den genererade HTML-koden är kompatibel med IE-webbläsaren. Standardvärdet är false. |
| [IsJsBrowserCompatible](../../aspose.cells/htmlsaveoptions/isjsbrowsercompatible/) { get; set; } | Anger om JavaScript är kompatibel med webbläsare som inte stödjer JavaScript. Standardvärdet är true. |
| [IsMobileCompatible](../../aspose.cells/htmlsaveoptions/ismobilecompatible/) { get; set; } | Anger om den genererade HTML-koden är kompatibel med mobila enheter. Standardvärdet är false. |
| [LayoutMode](../../aspose.cells/htmlsaveoptions/layoutmode/) { get; set; } | Hämtar eller anger layoutläge när du sparar till HTML. Standardvärdet är Normal |
| [LinkTargetType](../../aspose.cells/htmlsaveoptions/linktargettype/) { get; set; } | Anger typen av target-attribut i `<a>`-länk. Standardvärdet är HtmlLinkTargetType.Parent. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [MergeEmptyTdForcely](../../aspose.cells/htmlsaveoptions/mergeemptytdforcely/) { get; set; } | (**Obsolete.**) Anger om tomma TD-element ska slås ihop tvångsmässigt när filen exporteras till HTML. Storleken på HTML-filen minskar avsevärt när värdet sätts till true. Standardvärdet är false. Om du vill importera HTML-filen till Excel eller exportera perfekta rutnätslinjer när du sparar filen till HTML, behåll standardvärdet. |
| [MergeEmptyTdType](../../aspose.cells/htmlsaveoptions/mergeemptytdtype/) { get; set; } | Alternativet att slå ihop intilliggande tomma celler (tomma td-element). Standardvärdet är MergeEmptyTdType.Default. |
| [OfficeMathOutputMode](../../aspose.cells/htmlsaveoptions/officemathoutputmode/) { get; set; } | Anger hur OfficeMath-objekt exporteras till HTML, standardvärdet är Image. |
| [PageTitle](../../aspose.cells/htmlsaveoptions/pagetitle/) { get; set; } | Titeln på HTML-sidan. Endast för att spara till HTML-ström. |
| [ParseHtmlTagInCell](../../aspose.cells/htmlsaveoptions/parsehtmltagincell/) { get; set; } | Anger om HTML-taggar (såsom `<div></div>`) i en cell ska tolkas som cellvärde eller bevaras som de är. Standardvärdet är true. |
| [PresentationPreference](../../aspose.cells/htmlsaveoptions/presentationpreference/) { get; set; } | Anger om HTML- eller MHT-fil föredras för presentation. Standardvärdet är false. Om du vill ha en vackrare presentation, sätt värdet till true. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Anger om den senaste diagramdata ska cachas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SaveAsSingleFile](../../aspose.cells/htmlsaveoptions/saveassinglefile/) { get; set; } | Anger om HTML ska sparas som en enda fil. Standardvärdet är falskt. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Hämtar sparfilformatet. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SheetSet](../../aspose.cells/htmlsaveoptions/sheetset/) { get; set; } | Hämtar eller anger de blad som ska renderas. Standard är alla synliga blad i arbetsboken: [`Visible`](../../aspose.cells.rendering/sheetset/visible/). |
| [ShowAllSheets](../../aspose.cells/htmlsaveoptions/showallsheets/) { get; set; } | Anger om alla blad ska visas när man sparar som en enda HTML-fil. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Anger om externa definierade namn ska sorteras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Anger om definierade namn ska sorteras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [SpaceMode](../../aspose.cells/htmlsaveoptions/spacemode/) { get; set; } | Anger hur mellanslag renderas i HTML-utdata. Detta alternativ tillämpas för närvarande endast på numeriska format (t.ex. bokföringsformat). Standardvärdet är Css. |
| [StreamProvider](../../aspose.cells/htmlsaveoptions/streamprovider/) { get; set; } | Hämtar eller anger IStreamProvider för export av objekt. |
| [TableCssId](../../aspose.cells/htmlsaveoptions/tablecssid/) { get; set; } | Hämtar och anger prefixet för typ‑css‑namnet såsom tr, col, td osv, de finns i tabell‑elementet som har det specifika TableCssId‑attributet. Standardvärdet är "". |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Anger om inställning för smart art ska uppdateras. Standardvärdet är false. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Anger om sammanslagna celler ska valideras innan filen sparas. (Ärvd från [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Hämtar eller anger varningsåteranrop.(Ärvd från [`SaveOptions`](../saveoptions/).) |
| [WidthScalable](../../aspose.cells/htmlsaveoptions/widthscalable/) { get; set; } | Anger om kolumnbredd exporteras i skalenhet till HTML. Standardvärdet är falskt. |
| [WorksheetScalable](../../aspose.cells/htmlsaveoptions/worksheetscalable/) { get; set; } | Anger om HTML zoomas in eller ut via kalkylbladets zoomnivå när filen sparas till HTML, standardvärdet är falskt. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsDemo
    {
        public static void HtmlSaveOptionsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i kalkylbladet
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Skapa en instans av HtmlSaveOptions
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                IgnoreInvisibleShapes = true,
                PageTitle = "Sample HTML Page",
                AttachedFilesDirectory = "attached_files",
                AttachedFilesUrlPrefix = "http://example.com/files/",
                DefaultFontName = "Arial",
                AddGenericFont = true,
                WorksheetScalable = false,
                IsExportComments = false,
                ExportCommentsType = PrintCommentsType.PrintNoComments,
                DisableDownlevelRevealedComments = false,
                IsExpImageToTempDir = false,
                ImageScalable = true,
                WidthScalable = false,
                ExportSingleTab = false,
                ExportImagesAsBase64 = false,
                ExportActiveWorksheetOnly = false,
                ExportPrintAreaOnly = false,
                ExportArea = new CellArea { StartRow = 0, EndRow = 1, StartColumn = 0, EndColumn = 1 },
                ParseHtmlTagInCell = true,
                HtmlCrossStringType = HtmlCrossType.Default,
                HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden,
                HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden,
                Encoding = System.Text.Encoding.UTF8,
                SaveAsSingleFile = false,
                ShowAllSheets = false,
                ExportPageHeaders = false,
                ExportPageFooters = false,
                ExportHiddenWorksheet = true,
                PresentationPreference = false,
                CellCssPrefix = "",
                TableCssId = "",
                IsFullPathLink = false,
                ExportWorksheetCSSSeparately = false,
                ExportSimilarBorderStyle = false,
                MergeEmptyTdForcely = false,
                MergeEmptyTdType = MergeEmptyTdType.Default,
                ExportCellCoordinate = false,
                ExportExtraHeadings = false,
                ExportHeadings = false,
                ExportRowColumnHeadings = false,
                ExportFormula = true,
                AddTooltipText = false,
                ExportGridLines = false,
                ExportBogusRowData = true,
                ExcludeUnusedStyles = true,
                ExportDocumentProperties = true,
                ExportWorksheetProperties = true,
                ExportWorkbookProperties = true,
                ExportFrameScriptsAndProperties = true,
                ExportDataOptions = HtmlExportDataOptions.All,
                LinkTargetType = HtmlLinkTargetType.Parent,
                IsIECompatible = false,
                FormatDataIgnoreColumnWidth = false,
                CalculateFormula = true,
                IsJsBrowserCompatible = true,
                IsMobileCompatible = false,
                CssStyles = "body { padding: 5px }",
                HideOverflowWrappedText = false,
                IsBorderCollapsed = true,
                ClearData = false,
                CachedFileFolder = "cache",
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = true,
                SortExternalNames = true,
                RefreshChartCache = true,
                UpdateSmartArt = false
            };

            // Spara arbetsboken som HTML
            workbook.Save("HtmlSaveOptionsExample.html", saveOptions);

            return;
        }
    }
}
```

### Se även

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


