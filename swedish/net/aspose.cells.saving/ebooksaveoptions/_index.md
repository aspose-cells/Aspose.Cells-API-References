---
title: "Klass EbookSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Saving.EbookSaveOptions-klass. Representerar alternativen för att spara e‑bokfil"
type: docs
url: /sv/net/aspose.cells.saving/ebooksaveoptions/
---
## EbookSaveOptions class

Representerar alternativen för att spara e-bokfil.

```csharp
public class EbookSaveOptions : HtmlSaveOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [EbookSaveOptions](ebooksaveoptions/#constructor)() | Skapar alternativ för att spara e‑bokfil. |
| [EbookSaveOptions](ebooksaveoptions/#constructor_1)(SaveFormat) | Skapar alternativ för att spara e‑bokfil. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AddGenericFont](../../aspose.cells/htmlsaveoptions/addgenericfont/) { get; set; } | Anger om en generisk teckensnitt ska läggas till i CSS font-family. Standardvärdet är true (ärvt från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [AddTooltipText](../../aspose.cells/htmlsaveoptions/addtooltiptext/) { get; set; } | Anger om verktygstipstext ska läggas till när data inte kan visas helt. Standardvärdet är false. (Ärvt från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [AttachedFilesDirectory](../../aspose.cells/htmlsaveoptions/attachedfilesdirectory/) { get; set; } | Den katalog som de bifogade filerna kommer att sparas till. Endast för att spara till html‑ström. (Ärvt från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [AttachedFilesUrlPrefix](../../aspose.cells/htmlsaveoptions/attachedfilesurlprefix/) { get; set; } | Ange URL‑prefixet för bifogade filer såsom bild i html‑filen. Endast för att spara till html‑ström. (Ärvt från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Mappen för temporära filer som kan användas som datacache. (Ärvt från [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CalculateFormula](../../aspose.cells/htmlsaveoptions/calculateformula/) { get; set; } | Anger om formler ska beräknas innan html‑filen sparas. (Ärvt från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CellCssPrefix](../../aspose.cells/htmlsaveoptions/cellcssprefix/) { get; set; } | Hämtar och anger prefixet för css‑namnet, standardvärdet är "". (Ärvt från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CellNameAttribute](../../aspose.cells/htmlsaveoptions/cellnameattribute/) { get; set; } | Anger attributet som indikerar CellName att skrivas. (t.ex. Om värdet är "id", så blir utdata för cell "A1": &lt;td id='A1'&gt;). Standardvärdet är null. (Ärvt från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Om restriktioner i Excel‑filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32 K. När du matar in ett värde längre än 32 K kommer det att trunkeras. (Ärvt från [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Gör arbetsboken tom efter att filen har sparats. (Ärvt från [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Om true och katalogen inte finns kommer katalogen att skapas automatiskt innan filen sparas. (Ärvt från [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CssStyles](../../aspose.cells/htmlsaveoptions/cssstyles/) { get; set; } | Hämtar eller anger ytterligare css‑stilar för formateraren. Fungerar endast när [`SaveAsSingleFile`](../../aspose.cells/htmlsaveoptions/saveassinglefile/) är True.  CssStyles="body { padding: 5px }"; (Ärvt från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DataBarRenderMode](../../aspose.cells/htmlsaveoptions/databarrendermode/) { get; set; } | Representerar läget för hur DataBar renderas när Excel‑filer konverteras till html‑filer. Standardvärdet är BackgroundColor. (Ärvt från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DefaultFontName](../../aspose.cells/htmlsaveoptions/defaultfontname/) { get; set; } | Ange standardteckensnittets namn för export av html, standardteckensnittet kommer att användas när stilens teckensnitt inte finns, om denna egenskap är null kommer Aspose.Cells att använda ett universellt teckensnitt som har samma familj som originalteckensnittet, standardvärdet är null. (Ärvt från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DisableCss](../../aspose.cells/htmlsaveoptions/disablecss/) { get; set; } | Anger om endast inline‑stilar ska tillämpas, utan att förlita sig på CSS. Standardvärdet är false. (Ärvt från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DisableDownlevelRevealedComments](../../aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments/) { get; set; } | Anger om Downlevel-revealed villkorliga kommentarer ska inaktiveras vid export av fil till html, standardvärdet är falskt.(Ärvd från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EmbeddedFontType](../../aspose.cells/htmlsaveoptions/embeddedfonttype/) { get; set; } | Hämtar eller anger typen av inbäddning av teckensnittsfiler i html-filen. Standardvärdet är None vilket indikerar att inget teckensnitt kommer att bäddas in i html.(Ärvd från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EnableCssCustomProperties](../../aspose.cells/htmlsaveoptions/enablecsscustomproperties/) { get; set; } | Optimera html-utdata genom att använda anpassade CSS-egenskaper. Till exempel, i scenariot där det finns flera förekomster av en base64-bild, behöver bilddata med en anpassad egenskap bara sparas en gång, så prestandan för den resulterande html-filen kan förbättras. Standardvärdet är falskt.(Ärvd från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EncodeEntityAsCode](../../aspose.cells/htmlsaveoptions/encodeentityascode/) { get; set; } | Anger om html-teckenentiteter ska ersättas med decimalkod. (t.ex. \"&amp;nbsp;\" ersätts med \"&amp;#160;\"). Standardvärdet är falskt.(Ärvd från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [Encoding](../../aspose.cells/htmlsaveoptions/encoding/) { get; set; } | Om inte angivet används Encoding.UTF8 som standardkodningstyp.(Ärvd från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Anger om dokumentegenskaper ska krypteras vid sparande som .xls-fil. Standardvärdet är sant.(Ärvd från [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ExcludeUnusedStyles](../../aspose.cells/htmlsaveoptions/excludeunusedstyles/) { get; set; } | Anger om oanvända stilar ska uteslutas. För de genererade html-filerna kan uteslutning av oanvända stilar göra filstorleken mindre utan att påverka den visuella effekten. Så standardvärdet för denna egenskap är sant. Om användaren behöver behålla alla stilar i arbetsboken för den genererade html:n (t.ex. i scenariot där användaren senare ska återställa arbetsboken från den genererade html:n), sätt denna egenskap till falskt.(Ärvd från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportActiveWorksheetOnly](../../aspose.cells/htmlsaveoptions/exportactiveworksheetonly/) { get; set; } | Anger om endast det aktiva kalkylbladet ska exporteras till html-fil. Om sant exporteras bara det aktiva kalkylbladet till html-fil; om falskt exporteras hela arbetsboken till html-fil. Standardvärdet är falskt.(Ärvd från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportArea](../../aspose.cells/htmlsaveoptions/exportarea/) { get; set; } | Hämtar eller anger det exporterade CellArea för det aktuella aktiva kalkylbladet. Om du anger detta attribut kommer utskriftsområdet för det aktuella aktiva kalkylbladet att utelämnas. Endast det specificerade området exporteras när filen sparas till html.(Ärvd från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportBogusRowData](../../aspose.cells/htmlsaveoptions/exportbogusrowdata/) { get; set; } | Anger om falsk sista rad-data ska exporteras. Standardvärdet är sant. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet.(Ärvd från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportCellCoordinate](../../aspose.cells/htmlsaveoptions/exportcellcoordinate/) { get; set; } | Anger om Excel-koordinater för icke-tomma celler ska exporteras när filen sparas till html. Standardvärdet är falskt. Om du vill importera den genererade html-filen till Excel, behåll standardvärdet.(Ärvd från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportCommentsType](../../aspose.cells/htmlsaveoptions/exportcommentstype/) { get; set; } | Representerar typen av export av kommentarer till html-filer.(Ärvd från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportDataOptions](../../aspose.cells/htmlsaveoptions/exportdataoptions/) { get; set; } | Anger regeln för export av html-fildata. Standardvärdet är Alla.(Ärvd från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportDocumentProperties](../../aspose.cells/htmlsaveoptions/exportdocumentproperties/) { get; set; } | Anger om dokumentegenskaper ska exporteras. Standardvärdet är true. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportExtraHeadings](../../aspose.cells/htmlsaveoptions/exportextraheadings/) { get; set; } | Anger om extra rubriker ska exporteras när textlängden är längre än maxvisningskolumnen. Standardvärdet är false. Om du vill importera html-filen till Excel, behåll standardvärdet. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportFormula](../../aspose.cells/htmlsaveoptions/exportformula/) { get; set; } | Anger om formler ska exporteras när filen sparas till html. Standardvärdet är true. Om du vill importera den genererade html-filen till Excel, behåll standardvärdet. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportFrameScriptsAndProperties](../../aspose.cells/htmlsaveoptions/exportframescriptsandproperties/) { get; set; } | Anger om ram‑skript och dokumentegenskaper ska exporteras. Standardvärdet är true. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportGridLines](../../aspose.cells/htmlsaveoptions/exportgridlines/) { get; set; } | Anger om rutnätslinjer ska exporteras. Standardvärdet är false. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportHeadings](../../aspose.cells/htmlsaveoptions/exportheadings/) { get; set; } | (**Obsolete.**) Anger om bladets rad- och kolumnrubriker exporteras när du sparar till HTML-filer. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportHiddenWorksheet](../../aspose.cells/htmlsaveoptions/exporthiddenworksheet/) { get; set; } | Anger om dolda kalkylbladsinnehåll ska exporteras. Standardvärdet är true. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportImagesAsBase64](../../aspose.cells/htmlsaveoptions/exportimagesasbase64/) { get; set; } | Anger om bilder sparas i Base64-format till HTML, MHTML eller EPUB. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportNamedRangeAnchors](../../aspose.cells/htmlsaveoptions/exportnamedrangeanchors/) { get; set; } | Anger om ankarelement för namngivna områden ska exporteras när du sparar som HTML. Standardvärdet är true. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportObjectListener](../../aspose.cells/htmlsaveoptions/exportobjectlistener/) { get; set; } | (**Obsolete.**) Hämtar eller anger ExportObjectListener för export av objekt. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportPageFooters](../../aspose.cells/htmlsaveoptions/exportpagefooters/) { get; set; } | Anger om sidhuvuden ska exporteras. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportPageHeaders](../../aspose.cells/htmlsaveoptions/exportpageheaders/) { get; set; } | Anger om sidhuvuden ska exporteras. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportPrintAreaOnly](../../aspose.cells/htmlsaveoptions/exportprintareaonly/) { get; set; } | Anger om endast utskriftsområdet ska exporteras till html-filen. Standardvärdet är false. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportRowColumnHeadings](../../aspose.cells/htmlsaveoptions/exportrowcolumnheadings/) { get; set; } | Anger om bladets rad- och kolumnrubriker exporteras när du sparar till HTML-filer. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportSimilarBorderStyle](../../aspose.cells/htmlsaveoptions/exportsimilarborderstyle/) { get; set; } | Anger om liknande ramstil ska exporteras när ramstilen inte stöds av webbläsare. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet. Standardvärdet är false. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportSingleTab](../../aspose.cells/htmlsaveoptions/exportsingletab/) { get; set; } | Anger om den enda fliken ska exporteras när filen bara har ett kalkylblad. Standardvärdet är false. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportWorkbookProperties](../../aspose.cells/htmlsaveoptions/exportworkbookproperties/) { get; set; } | Anger om arbetsboks egenskaper ska exporteras. Standardvärdet är true. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet. (Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportWorksheetCSSSeparately](../../aspose.cells/htmlsaveoptions/exportworksheetcssseparately/) { get; set; } | Anger om kalkylbladets CSS ska exporteras separat. Standardvärdet är false. (Ärvd från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportWorksheetProperties](../../aspose.cells/htmlsaveoptions/exportworksheetproperties/) { get; set; } | Anger om kalkylbladets egenskaper ska exporteras. Standardvärdet är true. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet. (Ärvd från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [FilePathProvider](../../aspose.cells/htmlsaveoptions/filepathprovider/) { get; set; } | Hämtar eller anger IFilePathProvider för att exportera kalkylblad till html separat. (Ärvd från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [FormatDataIgnoreColumnWidth](../../aspose.cells/htmlsaveoptions/formatdataignorecolumnwidth/) { get; set; } | Anger om hela den formaterade celldata ska visas när den överskrider kolumnen. Om true ignoreras kolumnbredden och hela cellens data exporteras. Om false exporteras data på samma sätt som i Excel. Standardvärdet är false. (Ärvd från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HiddenColDisplayType](../../aspose.cells/htmlsaveoptions/hiddencoldisplaytype/) { get; set; } | Dold kolumn (bredden på denna kolumn är 0) i Excel, innan den sparas i html-format, om HtmlHiddenColDisplayType är \"Remove\" kommer den dolda kolumnen inte att skrivas ut, om värdet är \"Hidden\" kommer kolumnen att skrivas ut men vara dold, standardvärdet är \"Hidden\" (Ärvd från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HiddenRowDisplayType](../../aspose.cells/htmlsaveoptions/hiddenrowdisplaytype/) { get; set; } | Dold rad (höjden på denna rad är 0) i Excel, innan den sparas i html-format, om HtmlHiddenRowDisplayType är \"Remove\" kommer den dolda raden inte att skrivas ut, om värdet är \"Hidden\" kommer raden att skrivas ut men vara dold, standardvärdet är \"Hidden\" (Ärvd från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HideOverflowWrappedText](../../aspose.cells/htmlsaveoptions/hideoverflowwrappedtext/) { get; set; } | Anger om överskjutande text ska döljas när cellformatet är satt till radbrytning. Standardvärdet är false (Ärvd från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HtmlCrossStringType](../../aspose.cells/htmlsaveoptions/htmlcrossstringtype/) { get; set; } | Anger om en sträng som sträcker sig över flera celler ska visas på samma sätt som i MS Excel när en Excel-fil sparas i html-format. Som standard är värdet Default, så för strängar som sträcker sig över celler är skillnaden mellan html-filerna som skapas av Aspose.Cells och MS Excel liten. Men prestandan för att skapa stora html-filer blir flera gånger snabbare om värdet sätts till Cross jämfört med Default eller Fit2Cell. (Ärvd från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HtmlVersion](../../aspose.cells/htmlsaveoptions/htmlversion/) { get; set; } | Anger vilken version av HTML-standarden som ska användas när HTML-formatet sparas. Standardvärdet är HtmlVersion.Default. (Ärvd från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IgnoreInvisibleShapes](../../aspose.cells/htmlsaveoptions/ignoreinvisibleshapes/) { get; set; } | Anger om osynliga former ska exporteras (Ärvd från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ImageOptions](../../aspose.cells/htmlsaveoptions/imageoptions/) { get; } | Hämta ImageOrPrintOptions-objektet innan export (Ärvd från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ImageScalable](../../aspose.cells/htmlsaveoptions/imagescalable/) { get; set; } | Anger om skalbar enhet ska användas för att beskriva bildens bredd när skalbar enhet används för att beskriva kolumnbredden. Standardvärdet är true. (Ärvd från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsBorderCollapsed](../../aspose.cells/htmlsaveoptions/isbordercollapsed/) { get; set; } | Anger om tabellramarna är sammanslagna. Standardvärdet är true. (Ärvd från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsExpImageToTempDir](../../aspose.cells/htmlsaveoptions/isexpimagetotempdir/) { get; set; } | Anger om bildfiler ska exporteras till en temporär katalog. Endast för att spara till html-ström. (Ärvd från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsExportComments](../../aspose.cells/htmlsaveoptions/isexportcomments/) { get; set; } | Anger om kommentarer exporteras när fil sparas till html, standardvärdet är false.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsFullPathLink](../../aspose.cells/htmlsaveoptions/isfullpathlink/) { get; set; } | Anger om fullständig sökvägslänk används i sheet00x.htm, filelist.xml och tabstrip.htm. Standardvärdet är false.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsIECompatible](../../aspose.cells/htmlsaveoptions/isiecompatible/) { get; set; } | Anger om den genererade HTML är kompatibel med IE-webbläsaren. Standardvärdet är false(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsJsBrowserCompatible](../../aspose.cells/htmlsaveoptions/isjsbrowsercompatible/) { get; set; } | Anger om JavaScript är kompatibel med webbläsare som inte stödjer JavaScript. Standardvärdet är true.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsMobileCompatible](../../aspose.cells/htmlsaveoptions/ismobilecompatible/) { get; set; } | Anger om den genererade HTML är kompatibel med mobila enheter. Standardvärdet är false.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [LayoutMode](../../aspose.cells/htmlsaveoptions/layoutmode/) { get; set; } | Hämtar eller anger layoutläget när du sparar till HTML. Standardvärdet är Normal(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [LinkTargetType](../../aspose.cells/htmlsaveoptions/linktargettype/) { get; set; } | Anger typen av target-attribut i `<a>`-länken. Standardvärdet är HtmlLinkTargetType.Parent.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Anger om områdena för villkorsstyrd formatering och validering ska slås samman innan filen sparas.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [MergeEmptyTdForcely](../../aspose.cells/htmlsaveoptions/mergeemptytdforcely/) { get; set; } | (**Obsolete.**) Anger om tomma TD-element ska slås ihop tvångsmässigt vid export av fil till html. Storleken på html-filen minskar avsevärt efter att värdet satts till true. Standardvärdet är false. Om du vill importera html-filen till Excel eller exportera perfekta rutnätslinjer när du sparar fil till html, behåll standardvärdet.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [MergeEmptyTdType](../../aspose.cells/htmlsaveoptions/mergeemptytdtype/) { get; set; } | Alternativet för att slå samman intilliggande tomma celler (tomma td-element) Standardvärdet är MergeEmptyTdType.Default.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [OfficeMathOutputMode](../../aspose.cells/htmlsaveoptions/officemathoutputmode/) { get; set; } | Anger hur OfficeMath-objekt exporteras till HTML. Standardvärdet är Image.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [PageTitle](../../aspose.cells/htmlsaveoptions/pagetitle/) { get; set; } | Titeln på html-sidan. Endast för att spara till html-ström.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ParseHtmlTagInCell](../../aspose.cells/htmlsaveoptions/parsehtmltagincell/) { get; set; } | Anger om html-taggar (såsom `<div></div>`) i cellen ska tolkas som cellvärde eller bevaras som de är. Standardvärdet är true.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [PresentationPreference](../../aspose.cells/htmlsaveoptions/presentationpreference/) { get; set; } | Anger om html- eller mht-fil är presentationspreferens. Standardvärdet är false. Om du vill ha en vackrare presentation, sätt värdet till true.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Anger om den senaste datan för diagrammet ska cachas.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SaveAsSingleFile](../../aspose.cells/htmlsaveoptions/saveassinglefile/) { get; set; } | Anger om html ska sparas som en enda fil. Standardvärdet är false.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Hämtar filformatet för sparning.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SheetSet](../../aspose.cells/htmlsaveoptions/sheetset/) { get; set; } | Hämtar eller anger bladen som ska renderas. Standard är alla synliga blad i arbetsboken: [`Visible`](../../aspose.cells.rendering/sheetset/visible/).(Ärvt från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ShowAllSheets](../../aspose.cells/htmlsaveoptions/showallsheets/) { get; set; } | Anger om alla blad visas när du sparar som en enda html‑fil.(Ärvt från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Anger om externa definierade namn ska sorteras innan filen sparas.(Ärvt från [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Anger om definierade namn ska sorteras innan filen sparas.(Ärvt från [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SpaceMode](../../aspose.cells/htmlsaveoptions/spacemode/) { get; set; } | Anger hur mellanslag renderas i HTML‑utdata. Detta alternativ tillämpas för närvarande endast på numeriska format (t.ex. bokföringsformat). Standardvärdet är Css.(Ärvt från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [StreamProvider](../../aspose.cells/htmlsaveoptions/streamprovider/) { get; set; } | Hämtar eller anger IStreamProvider för att exportera objekt.(Ärvt från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [TableCssId](../../aspose.cells/htmlsaveoptions/tablecssid/) { get; set; } | Hämtar och anger prefixet för typ‑css‑namnet såsom tr, col, td osv., de finns i tabell‑elementet som har det specifika TableCssId‑attributet. Standardvärdet är "".(Ärvt från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Anger om inställning för smart art uppdateras. Standardvärdet är false.(Ärvt från [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Anger om sammanslagna celler ska valideras innan filen sparas.(Ärvt från [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Hämtar eller anger varnings‑callback.(Ärvt från [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [WidthScalable](../../aspose.cells/htmlsaveoptions/widthscalable/) { get; set; } | Anger om kolumnbredd exporteras i skalenhet till html. Standardvärdet är false.(Ärvt från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [WorksheetScalable](../../aspose.cells/htmlsaveoptions/worksheetscalable/) { get; set; } | Anger om html zoomas in eller ut via kalkylbladets zoomnivå när filen sparas till html, standardvärdet är false.(Ärvt från [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class EbookSaveOptionsDemo
    {
        public static void EbookSaveOptionsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello World");

            // Skapa en instans av EbookSaveOptions
            EbookSaveOptions saveOptions = new EbookSaveOptions();

            // Ställa in egenskaper
            saveOptions.IgnoreInvisibleShapes = true;
            saveOptions.PageTitle = "Sample Page Title";
            saveOptions.AttachedFilesDirectory = "attached_files";
            saveOptions.AttachedFilesUrlPrefix = "http://example.com/files/";
            saveOptions.DefaultFontName = "Arial";
            saveOptions.AddGenericFont = true;
            saveOptions.WorksheetScalable = false;
            saveOptions.IsExportComments = false;
            saveOptions.ExportCommentsType = PrintCommentsType.PrintNoComments;
            saveOptions.DisableDownlevelRevealedComments = false;
            saveOptions.IsExpImageToTempDir = false;
            saveOptions.ImageScalable = true;
            saveOptions.WidthScalable = false;
            saveOptions.ExportSingleTab = false;
            saveOptions.ExportImagesAsBase64 = false;
            saveOptions.ExportActiveWorksheetOnly = false;
            saveOptions.ExportPrintAreaOnly = false;
            saveOptions.ExportArea = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            saveOptions.ParseHtmlTagInCell = true;
            saveOptions.HtmlCrossStringType = HtmlCrossType.Default;
            saveOptions.HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden;
            saveOptions.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden;
            saveOptions.Encoding = System.Text.Encoding.UTF8;
            saveOptions.SaveAsSingleFile = false;
            saveOptions.ShowAllSheets = true;
            saveOptions.ExportPageHeaders = true;
            saveOptions.ExportPageFooters = true;
            saveOptions.ExportHiddenWorksheet = true;
            saveOptions.PresentationPreference = false;
            saveOptions.CellCssPrefix = "cell_";
            saveOptions.TableCssId = "table_";
            saveOptions.IsFullPathLink = false;
            saveOptions.ExportWorksheetCSSSeparately = false;
            saveOptions.ExportSimilarBorderStyle = false;
            saveOptions.MergeEmptyTdForcely = false;
            saveOptions.MergeEmptyTdType = MergeEmptyTdType.Default;
            saveOptions.ExportCellCoordinate = false;
            saveOptions.ExportExtraHeadings = false;
            saveOptions.ExportHeadings = true;
            saveOptions.ExportRowColumnHeadings = true;
            saveOptions.ExportFormula = true;
            saveOptions.AddTooltipText = false;
            saveOptions.ExportGridLines = false;
            saveOptions.ExportBogusRowData = true;
            saveOptions.ExcludeUnusedStyles = true;
            saveOptions.ExportDocumentProperties = true;
            saveOptions.ExportWorksheetProperties = true;
            saveOptions.ExportWorkbookProperties = true;
            saveOptions.ExportFrameScriptsAndProperties = true;
            saveOptions.ExportDataOptions = HtmlExportDataOptions.All;
            saveOptions.LinkTargetType = HtmlLinkTargetType.Parent;
            saveOptions.IsIECompatible = false;
            saveOptions.FormatDataIgnoreColumnWidth = false;
            saveOptions.CalculateFormula = true;
            saveOptions.IsJsBrowserCompatible = true;
            saveOptions.IsMobileCompatible = false;
            saveOptions.CssStyles = "body { padding: 5px }";
            saveOptions.HideOverflowWrappedText = false;
            saveOptions.IsBorderCollapsed = true;
            saveOptions.ClearData = true;
            saveOptions.CachedFileFolder = "cache";
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = true;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = true;
            saveOptions.RefreshChartCache = true;
            saveOptions.WarningCallback = null;
            saveOptions.UpdateSmartArt = true;

            // Spara arbetsboken till en HTML‑fil med de angivna alternativen
            workbook.Save("EbookSaveOptionsExample.html", saveOptions);

            return;
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../../aspose.cells/htmlsaveoptions/)
* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


