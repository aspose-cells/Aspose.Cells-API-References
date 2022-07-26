---
title: HtmlSaveOptions
second_title: Aspose.Cells för .NET API-referens
description: Representerar alternativen för att spara html-fil.
type: docs
weight: 3740
url: /sv/net/aspose.cells/htmlsaveoptions/
---
## HtmlSaveOptions class

Representerar alternativen för att spara html-fil.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions#constructor)() | Skapar alternativ för att spara html-fil. |
| [HtmlSaveOptions](htmlsaveoptions#constructor_1)(SaveFormat) | Skapar alternativ för att spara htm-fil. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [AddTooltipText](../../aspose.cells/htmlsaveoptions/addtooltiptext) { get; set; } | Indikerar om man lägger till verktygstipstext när data inte kan visas helt. Standardvärdet är false. |
| [AttachedFilesDirectory](../../aspose.cells/htmlsaveoptions/attachedfilesdirectory) { get; set; } | Mappen som de bifogade filerna kommer att sparas i. Endast för att spara till html-ström. |
| [AttachedFilesUrlPrefix](../../aspose.cells/htmlsaveoptions/attachedfilesurlprefix) { get; set; } | Ange URL-prefixet för bifogade filer såsom bild i html-filen. Endast för att spara till html-ström. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder) { get; set; } | Den cachade filmappen används för att lagra en del stora data. |
| [CellCssPrefix](../../aspose.cells/htmlsaveoptions/cellcssprefix) { get; set; } | Hämtar och ställer in prefixet för css-namnet, standardvärdet är "". |
| [ClearData](../../aspose.cells/saveoptions/cleardata) { get; set; } | Gör arbetsboken tom när du har sparat filen. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory) { get; set; } | Om true och katalogen inte finns skapas katalogen automatiskt innan filen sparas. |
| [DefaultFontName](../../aspose.cells/htmlsaveoptions/defaultfontname) { get; set; } | Ange standardteckensnittsnamnet för att exportera html, standardteckensnittet kommer att användas när stilteckensnittet inte finns, Om denna egenskap är null kommer Aspose.Cells att använda universella teckensnitt som har samma familj med det ursprungliga teckensnittet, standardvärdet är null. |
| [DisableDownlevelRevealedComments](../../aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments) { get; set; } | Indikerar om inaktivera Downlevel-avslöjade villkorliga kommentarer vid export av fil till html, standardvärdet är false. |
| [Encoding](../../aspose.cells/htmlsaveoptions/encoding) { get; set; } | Om inte inställt, använd Encoding.UTF8 som standardkodningstyp. |
| [ExcludeUnusedStyles](../../aspose.cells/htmlsaveoptions/excludeunusedstyles) { get; set; } | Anger om oanvända stilar utesluts. För de genererade html-filerna kan exkludering av oanvända stilar göra filstorleken mindre utan att påverka de visuella effekterna. Så standardvärdet för den här egenskapen är true. Om användaren behöver behålla alla stilar i arbetsboken för den genererade HTML-koden (t.ex. scenariot att user behöver återställa arbetsboken från den genererade HTML-koden senare), ställ in den här egenskapen som falsk . |
| [ExportActiveWorksheetOnly](../../aspose.cells/htmlsaveoptions/exportactiveworksheetonly) { get; set; } | Indikerar om hela arbetsboken exporteras till html-fil. |
| [ExportArea](../../aspose.cells/htmlsaveoptions/exportarea) { get; set; } | Hämtar eller ställer in det exporterande cellområdet för det aktuella aktiva kalkylbladet. Om du ställer in det här attributet kommer utskriftsområdet för det aktuella aktiva kalkylbladet att utelämnas. Endast det angivna området kommer att exporteras när filen sparas till html. |
| [ExportBogusRowData](../../aspose.cells/htmlsaveoptions/exportbogusrowdata) { get; set; } | Indikerar om falsk data på nedre raden exporteras. Standardvärdet är sant. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet. |
| [ExportCellCoordinate](../../aspose.cells/htmlsaveoptions/exportcellcoordinate) { get; set; } | Indikerar om export av excel-koordinater för icke-tomma celler när filen sparas till html. Standardvärdet är false. Om du vill importera utdata-html till Excel, behåll standardvärdet. |
| [ExportDataOptions](../../aspose.cells/htmlsaveoptions/exportdataoptions) { get; set; } | Indikerar regeln för export av html-fildata. Standardvärdet är All. |
| [ExportDocumentProperties](../../aspose.cells/htmlsaveoptions/exportdocumentproperties) { get; set; } | Indikerar om du exporterar dokumentegenskaper. Standardvärdet är sant. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet. |
| [ExportExtraHeadings](../../aspose.cells/htmlsaveoptions/exportextraheadings) { get; set; } | Indikerar om extra rubriker exporteras när textens längd är längre än max visningskolumnen. Standardvärdet är falskt. Om du vill importera html-filen till Excel, behåll standardvärdet. |
| [ExportFormula](../../aspose.cells/htmlsaveoptions/exportformula) { get; set; } | Indikerar om formeln exporteras när filen sparas till html. Standardvärdet är true. Om du vill importera utdata-html till Excel, behåll standardvärdet. |
| [ExportFrameScriptsAndProperties](../../aspose.cells/htmlsaveoptions/exportframescriptsandproperties) { get; set; } | Anger om ramskript och dokumentegenskaper exporteras. Standardvärdet är sant. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet. |
| [ExportGridLines](../../aspose.cells/htmlsaveoptions/exportgridlines) { get; set; } | Indikerar om rutnätslinjerna exporteras. Standardvärdet är false. |
| [ExportHiddenWorksheet](../../aspose.cells/htmlsaveoptions/exporthiddenworksheet) { get; set; } | Indikerar om det dolda kalkylbladets innehåll exporteras. Standardvärdet är sant. |
| [ExportImagesAsBase64](../../aspose.cells/htmlsaveoptions/exportimagesasbase64) { get; set; } | Anger om bilder sparas i Base64-format till HTML, MHTML eller EPUB. |
| [ExportPageFooters](../../aspose.cells/htmlsaveoptions/exportpagefooters) { get; set; } | Anger om sidhuvuden exporteras. |
| [ExportPageHeaders](../../aspose.cells/htmlsaveoptions/exportpageheaders) { get; set; } | Anger om sidhuvuden exporteras. |
| [ExportPrintAreaOnly](../../aspose.cells/htmlsaveoptions/exportprintareaonly) { get; set; } | Indikerar om utskriftsområdet endast exporteras till html-fil. Standardvärdet är false. |
| [ExportRowColumnHeadings](../../aspose.cells/htmlsaveoptions/exportrowcolumnheadings) { get; set; } | Anger om arkets rad- och kolumnrubriker exporteras när du sparar till HTML-filer. |
| [ExportSimilarBorderStyle](../../aspose.cells/htmlsaveoptions/exportsimilarborderstyle) { get; set; } | Anger om du exporterar liknande kantstil när kantstilen inte stöds av webbläsare. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet. Standardvärdet är false. |
| [ExportSingleTab](../../aspose.cells/htmlsaveoptions/exportsingletab) { get; set; } | Anger om den enskilda fliken exporteras när filen bara har ett kalkylblad. Standardvärdet är false. |
| [ExportWorkbookProperties](../../aspose.cells/htmlsaveoptions/exportworkbookproperties) { get; set; } | Anger om arbetsbokens egenskaper exporteras. Standardvärdet är sant. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet. |
| [ExportWorksheetCSSSeparately](../../aspose.cells/htmlsaveoptions/exportworksheetcssseparately) { get; set; } | Indikerar om kalkylbladets css exporteras separat. Standardvärdet är false. |
| [ExportWorksheetProperties](../../aspose.cells/htmlsaveoptions/exportworksheetproperties) { get; set; } | Indikerar om kalkylbladsegenskaper exporteras. Standardvärdet är sant. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet. |
| [FilePathProvider](../../aspose.cells/htmlsaveoptions/filepathprovider) { get; set; } | Hämtar eller ställer in IFilePathProvider för export av kalkylblad till html separat. |
| [HiddenColDisplayType](../../aspose.cells/htmlsaveoptions/hiddencoldisplaytype) { get; set; } | Hidden kolumn (bredden på denna kolumn är 0) i excel, innan du sparar denna i html-format, om HtmlHiddenColDisplayType är "Remove", skulle den dolda kolumnen inte matas ut, om värdet är "Hidden", skulle kolumnen har matats ut, men dolts, standardvärdet är "Hidden" |
| [HiddenRowDisplayType](../../aspose.cells/htmlsaveoptions/hiddenrowdisplaytype) { get; set; } | Hidden rad (höjden på denna rad är 0) i excel, innan du sparar detta i html-format, om HtmlHiddenRowDisplayType är "Remove", den dolda raden skulle inte matas ut, om värdet är "Hidden", skulle raden har matats ut, men dolts, standardvärdet är "Hidden" |
| [HtmlCrossStringType](../../aspose.cells/htmlsaveoptions/htmlcrossstringtype) { get; set; } | Indikerar om en korscellsträng kommer att visas på samma sätt som MS Excel när man sparar en Excel-fil i html-format. Som standard är värdet Default, så för korscellsträngar är det liten skillnad mellan html filer skapade av Aspose.Cells och MS Excel. Men prestandan för att skapa stora html-filer, inställning av värdet till Cross skulle vara flera gånger snabbare än att ställa in det till Default eller Fit2Cell. |
| [IgnoreInvisibleShapes](../../aspose.cells/htmlsaveoptions/ignoreinvisibleshapes) { get; set; } | Ange om export av de osynliga formerna |
| [ImageOptions](../../aspose.cells/htmlsaveoptions/imageoptions) { get; } | Hämta ImageOrPrintOptions-objektet innan du exporterar |
| [ImageScalable](../../aspose.cells/htmlsaveoptions/imagescalable) { get; set; } | Anger om skalbar enhet används för att beskriva bilden width när skalbar enhet används för att beskriva kolumnbredden. Standardvärdet är sant. |
| [IsExpImageToTempDir](../../aspose.cells/htmlsaveoptions/isexpimagetotempdir) { get; set; } | Anger om bildfiler exporteras till temporär katalog. Endast för att spara till HTML-ström. |
| [IsExportComments](../../aspose.cells/htmlsaveoptions/isexportcomments) { get; set; } | Indikerar om kommentarer exporteras när filen sparas till html, standardvärdet är false. |
| [IsFullPathLink](../../aspose.cells/htmlsaveoptions/isfullpathlink) { get; set; } | Indikerar om fullständig sökvägslänk används i sheet00x.htm,filelist.xml och tabstrip.htm. Standardvärdet är false. |
| [LinkTargetType](../../aspose.cells/htmlsaveoptions/linktargettype) { get; set; } | Indikerar typen av målattribut i &lt;a&gt;-länken. Standardvärdet är HtmlLinkTargetType.Parent. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas) { get; set; } | Anger om områdena för villkorlig formatering och validering slås samman innan filen sparas. |
| [MergeEmptyTdForcely](../../aspose.cells/htmlsaveoptions/mergeemptytdforcely) { get; set; } | Indikerar om sammanslagning av tomt TD-element tvingas vid export av fil till html. Storleken på html-filen kommer att minskas avsevärt efter att värdet satts till sant. Standardvärdet är falskt. Om du vill importera html-filen till Excel eller exportera perfekta rutnätslinjer när du sparar filen till html, behåll standardvärdet. |
| [PageTitle](../../aspose.cells/htmlsaveoptions/pagetitle) { get; set; } | Titeln på HTML-sidan. Endast för att spara till HTML-ström. |
| [ParseHtmlTagInCell](../../aspose.cells/htmlsaveoptions/parsehtmltagincell) { get; set; } | Analysera HTML-tagg i cell, som ,som cellvärde,eller som html-tagg,standard är true |
| [PresentationPreference](../../aspose.cells/htmlsaveoptions/presentationpreference) { get; set; } | Indikerar om html- eller mht-fil är presentationspreferens. Standardvärdet är false. Om du vill få en vackrare presentation, ställ in värdet till true. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache) { get; set; } | Indikerar om uppdatering av diagramcachedata |
| [SaveAsSingleFile](../../aspose.cells/htmlsaveoptions/saveassinglefile) { get; set; } | Indikerar om HTML-filen sparas som en enda fil. Standardvärdet är false. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat) { get; } | Hämtar spara filformatet. |
| [ShowAllSheets](../../aspose.cells/htmlsaveoptions/showallsheets) { get; set; } | Indikerar om alla ark visas när du sparar som en enda html-fil. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames) { get; set; } | Indikerar om externt definierade namn sorteras innan filen sparas. |
| [SortNames](../../aspose.cells/saveoptions/sortnames) { get; set; } | Indikerar om du sorterar definierade namn innan filen sparas. |
| [StreamProvider](../../aspose.cells/htmlsaveoptions/streamprovider) { get; set; } | Hämtar eller ställer in IStreamProvider för export av objekt. |
| [TableCssId](../../aspose.cells/htmlsaveoptions/tablecssid) { get; set; } | Hämtar och ställer in prefixet för typen css-namn som tr,col,td och så vidare, de finns i tabellelementet som har det specifika TableCssId-attributet. Standardvärdet är "". |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart) { get; set; } | Indikerar om uppdatering av smart art-inställning. Standardvärdet är false. |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas) { get; set; } | Anger om validera sammanslagna celler innan filen sparas. |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback) { get; set; } | Får eller ställer in varningsåteruppringning. |
| [WidthScalable](../../aspose.cells/htmlsaveoptions/widthscalable) { get; set; } | Anger om skalbar enhet används för att beskriva kolumnbredden vid export av fil till html. Standardvärdet är false. |
| [WorksheetScalable](../../aspose.cells/htmlsaveoptions/worksheetscalable) { get; set; } | Indikerar om du zoomar in eller ut html via kalkylbladszoomnivå när du sparar fil till html, standardvärdet är false. |

### Se även

* class [SaveOptions](../saveoptions)
* namnutrymme [Aspose.Cells](../../aspose.cells)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
