---
title: "EbookSaveOptions klass"
linktitle: "EbookSaveOptions"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "EbookSaveOptions-klass. Inkapslar objektet som representerar ebooksaveoptions i Go."
type: docs
weight: 200
url: /sv/go-cpp/ebooksaveoptions/
---

## EbookSaveOptions class

Representerar alternativen för att spara e-bokfilen.

```go

type EbookSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewEbookSaveOptions](./newebooksaveoptions/) | Skapar alternativ för att spara e-bokfil. |
| [NewEbookSaveOptions_SaveFormat](./newebooksaveoptions_saveformat/) | Skapar alternativ för att spara e-bokfil. |
| [NewEbookSaveOptions_HtmlSaveOptions](./newebooksaveoptions_htmlsaveoptions/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetIgnoreInvisibleShapes](./getignoreinvisibleshapes/) | Anger om osynliga former ska exporteras |
| [SetIgnoreInvisibleShapes](./setignoreinvisibleshapes/) | Anger om osynliga former ska exporteras |
| [GetPageTitle](./getpagetitle/) | Titeln på HTML-sidan. Endast för att spara till HTML-ström. |
| [SetPageTitle](./setpagetitle/) | Titeln på HTML-sidan. Endast för att spara till HTML-ström. |
| [GetAttachedFilesDirectory](./getattachedfilesdirectory/) | Den katalog som de bifogade filerna kommer att sparas i.Endast för att spara till html‑ström. |
| [SetAttachedFilesDirectory](./setattachedfilesdirectory/) | Den katalog som de bifogade filerna kommer att sparas i.Endast för att spara till html‑ström. |
| [GetAttachedFilesUrlPrefix](./getattachedfilesurlprefix/) | Ange URL‑prefixet för bifogade filer, såsom bild i html‑filen.Endast för att spara till html‑ström. |
| [SetAttachedFilesUrlPrefix](./setattachedfilesurlprefix/) | Ange URL‑prefixet för bifogade filer, såsom bild i html‑filen.Endast för att spara till html‑ström. |
| [GetDefaultFontName](./getdefaultfontname/) | Ange standardteckensnittets namn för export av html, standardteckensnittet kommer att användas när stilens teckensnitt inte finns. Om detta egenskap är null kommer Aspose.Cells att använda ett universellt teckensnitt som har samma familj som originalteckensnittet, standardvärdet är null. |
| [SetDefaultFontName](./setdefaultfontname/) | Ange standardteckensnittets namn för export av html, standardteckensnittet kommer att användas när stilens teckensnitt inte finns. Om detta egenskap är null kommer Aspose.Cells att använda ett universellt teckensnitt som har samma familj som originalteckensnittet, standardvärdet är null. |
| [GetAddGenericFont](./getaddgenericfont/) | Anger om en generisk teckensnitt ska läggas till i CSS font-family.Standardvärdet är true. |
| [SetAddGenericFont](./setaddgenericfont/) | Anger om en generisk teckensnitt ska läggas till i CSS font-family.Standardvärdet är true. |
| [GetWorksheetScalable](./getworksheetscalable/) | Anger om zoomning in eller out av html via kalkylbladets zoomnivå när filen sparas till html, standardvärdet är false. |
| [SetWorksheetScalable](./setworksheetscalable/) | Anger om zoomning in eller out av html via kalkylbladets zoomnivå när filen sparas till html, standardvärdet är false. |
| [IsExportComments](./isexportcomments/) | Anger om kommentarer exporteras när filen sparas till html, standardvärdet är false. |
| [SetIsExportComments](./setisexportcomments/) | Anger om kommentarer exporteras när filen sparas till html, standardvärdet är false. |
| [GetExportCommentsType](./getexportcommentstype/) | Representerar typ av export av kommentarer till html‑filer. |
| [SetExportCommentsType](./setexportcommentstype/) | Representerar typ av export av kommentarer till html‑filer. |
| [GetDisableDownlevelRevealedComments](./getdisabledownlevelrevealedcomments/) | Anger om Downlevel‑revealed villkorliga kommentarer ska inaktiveras vid export av fil till html, standardvärdet är false. |
| [SetDisableDownlevelRevealedComments](./setdisabledownlevelrevealedcomments/) | Anger om Downlevel‑revealed villkorliga kommentarer ska inaktiveras vid export av fil till html, standardvärdet är false. |
| [IsExpImageToTempDir](./isexpimagetotempdir/) | Anger om bildfiler exporteras till temporärkatalogen.Endast för att spara till html‑ström. |
| [SetIsExpImageToTempDir](./setisexpimagetotempdir/) | Anger om bildfiler exporteras till temporärkatalogen.Endast för att spara till html‑ström. |
| [GetImageScalable](./getimagescalable/) | Anger om skalbar enhet används för att beskriva bildens bredd när skalbar enhet används för att beskriva kolumnens bredd. Standardvärdet är true. |
| [SetImageScalable](./setimagescalable/) | Anger om skalbar enhet används för att beskriva bildens bredd när skalbar enhet används för att beskriva kolumnens bredd. Standardvärdet är true. |
| [GetWidthScalable](./getwidthscalable/) | Anger om kolumnbredd exporteras i skalenhet till html.Standardvärdet är false. |
| [SetWidthScalable](./setwidthscalable/) | Anger om kolumnbredd exporteras i skalenhet till html.Standardvärdet är false. |
| [GetExportSingleTab](./getexportsingletab/) | Anger om den enda fliken exporteras när filen bara har ett kalkylblad.Standardvärdet är false. |
| [SetExportSingleTab](./setexportsingletab/) | Anger om den enda fliken exporteras när filen bara har ett kalkylblad.Standardvärdet är false. |
| [GetExportImagesAsBase64](./getexportimagesasbase64/) | Anger om bilder sparas i Base64‑format till HTML, MHTML eller EPUB. |
| [SetExportImagesAsBase64](./setexportimagesasbase64/) | Anger om bilder sparas i Base64‑format till HTML, MHTML eller EPUB. |
| [GetExportActiveWorksheetOnly](./getexportactiveworksheetonly/) | Anger om endast det aktiva kalkylbladet ska exporteras till html‑filen.Om true exporteras bara det aktiva kalkylbladet till html‑filen;Om false exporteras hela arbetsboken till html‑filen.Standardvärdet är false. |
| [SetExportActiveWorksheetOnly](./setexportactiveworksheetonly/) | Anger om endast det aktiva kalkylbladet ska exporteras till html‑filen.Om true exporteras bara det aktiva kalkylbladet till html‑filen;Om false exporteras hela arbetsboken till html‑filen.Standardvärdet är false. |
| [GetExportPrintAreaOnly](./getexportprintareaonly/) | Anger om endast utskriftsområdet ska exporteras till html‑filen. Standardvärdet är false. |
| [SetExportPrintAreaOnly](./setexportprintareaonly/) | Anger om endast utskriftsområdet ska exporteras till html‑filen. Standardvärdet är false. |
| [GetExportArea](./getexportarea/) | Hämtar eller anger det exporterade CellArea för det aktuella aktiva Worksheet.Om du anger detta attribut kommer utskriftsområdet för det aktuella aktiva Worksheet att utelämnas. Endast det specificerade området exporteras när filen sparas till html. |
| [SetExportArea](./setexportarea/) | Hämtar eller anger det exporterade CellArea för det aktuella aktiva Worksheet.Om du anger detta attribut kommer utskriftsområdet för det aktuella aktiva Worksheet att utelämnas. Endast det specificerade området exporteras när filen sparas till html. |
| [GetParseHtmlTagInCell](./getparsehtmltagincell/) | Anger om html‑taggar (såsom <c>&lt;div&gt;&lt;/div&gt;</c>) i en cell ska tolkas som cellvärde eller bevaras som de är.Standardvärdet är true. |
| [SetParseHtmlTagInCell](./setparsehtmltagincell/) | Anger om html‑taggar (såsom <c>&lt;div&gt;&lt;/div&gt;</c>) i en cell ska tolkas som cellvärde eller bevaras som de är.Standardvärdet är true. |
| [GetHtmlCrossStringType](./gethtmlcrossstringtype/) | Anger om en sträng som sträcker sig över flera celler visas på samma sätt som i MS Excel när en Excel‑fil sparas i html‑format. Som standard är värdet Default, så för strängar som sträcker sig över celler är skillnaden mellan html‑filer skapade av Aspose.Cells och MS Excel liten. Men prestandan för att skapa stora html‑filer blir flera gånger snabbare om värdet sätts till Cross jämfört med Default eller Fit2Cell. |
| [SetHtmlCrossStringType](./sethtmlcrossstringtype/) | Anger om en sträng som sträcker sig över flera celler visas på samma sätt som i MS Excel när en Excel‑fil sparas i html‑format. Som standard är värdet Default, så för strängar som sträcker sig över celler är skillnaden mellan html‑filer skapade av Aspose.Cells och MS Excel liten. Men prestandan för att skapa stora html‑filer blir flera gånger snabbare om värdet sätts till Cross jämfört med Default eller Fit2Cell. |
| [GetHiddenColDisplayType](./gethiddencoldisplaytype/) | Dold kolumn (bredden på denna kolumn är 0) i Excel, innan den sparas i html‑format, om HtmlHiddenColDisplayType är \"Remove\" kommer den dolda kolumnen inte att skrivas ut, om värdet är \"Hidden\" kommer kolumnen att skrivas ut men vara dold, standardvärdet är \"Hidden\". |
| [SetHiddenColDisplayType](./sethiddencoldisplaytype/) | Dold kolumn (bredden på denna kolumn är 0) i Excel, innan den sparas i html‑format, om HtmlHiddenColDisplayType är \"Remove\" kommer den dolda kolumnen inte att skrivas ut, om värdet är \"Hidden\" kommer kolumnen att skrivas ut men vara dold, standardvärdet är \"Hidden\". |
| [GetHiddenRowDisplayType](./gethiddenrowdisplaytype/) | Dold rad (höjden på denna rad är 0) i Excel, innan den sparas i html‑format, om HtmlHiddenRowDisplayType är \"Remove\" kommer den dolda raden inte att skrivas ut, om värdet är \"Hidden\" kommer raden att skrivas ut men vara dold, standardvärdet är \"Hidden\". |
| [SetHiddenRowDisplayType](./sethiddenrowdisplaytype/) | Dold rad (höjden på denna rad är 0) i Excel, innan den sparas i html‑format, om HtmlHiddenRowDisplayType är \"Remove\" kommer den dolda raden inte att skrivas ut, om värdet är \"Hidden\" kommer raden att skrivas ut men vara dold, standardvärdet är \"Hidden\". |
| [GetEncoding](./getencoding/) | Om inte angivet, använd Encoding.UTF8 som standardkodningstyp. |
| [SetEncoding](./setencoding/) | Om inte angivet, använd Encoding.UTF8 som standardkodningstyp. |
| [GetImageOptions](./getimageoptions/) | Hämta ImageOrPrintOptions‑objektet innan export. |
| [GetSaveAsSingleFile](./getsaveassinglefile/) | Anger om HTML ska sparas som en enda fil. Standardvärdet är falskt. |
| [SetSaveAsSingleFile](./setsaveassinglefile/) | Anger om HTML ska sparas som en enda fil. Standardvärdet är falskt. |
| [GetShowAllSheets](./getshowallsheets/) | Anger om alla blad ska visas när de sparas som en enda HTML-fil. |
| [SetShowAllSheets](./setshowallsheets/) | Anger om alla blad ska visas när de sparas som en enda HTML-fil. |
| [GetExportPageHeaders](./getexportpageheaders/) | Anger om sidhuvuden ska exporteras. |
| [SetExportPageHeaders](./setexportpageheaders/) | Anger om sidhuvuden ska exporteras. |
| [GetExportPageFooters](./getexportpagefooters/) | Anger om sidhuvuden ska exporteras. |
| [SetExportPageFooters](./setexportpagefooters/) | Anger om sidhuvuden ska exporteras. |
| [GetExportHiddenWorksheet](./getexporthiddenworksheet/) | Anger om dolda arbetsbladsinnehåll ska exporteras. Standardvärdet är sant. |
| [SetExportHiddenWorksheet](./setexporthiddenworksheet/) | Anger om dolda arbetsbladsinnehåll ska exporteras. Standardvärdet är sant. |
| [GetPresentationPreference](./getpresentationpreference/) | Anger om HTML- eller MHT-fil är presentationspreferens. Standardvärdet är falskt. Om du vill ha en vackrare presentation, sätt värdet till sant. |
| [SetPresentationPreference](./setpresentationpreference/) | Anger om HTML- eller MHT-fil är presentationspreferens. Standardvärdet är falskt. Om du vill ha en vackrare presentation, sätt värdet till sant. |
| [GetCellCssPrefix](./getcellcssprefix/) | Hämtar och anger prefixet för CSS-namnet, standardvärdet är "". |
| [SetCellCssPrefix](./setcellcssprefix/) | Hämtar och anger prefixet för CSS-namnet, standardvärdet är "". |
| [GetTableCssId](./gettablecssid/) | Hämtar och anger prefixet för typ-CSS-namn såsom tr, col, td osv, som finns i tabell‑elementet som har det specifika TableCssId‑attributet. Standardvärdet är "". |
| [SetTableCssId](./settablecssid/) | Hämtar och anger prefixet för typ-CSS-namn såsom tr, col, td osv, som finns i tabell‑elementet som har det specifika TableCssId‑attributet. Standardvärdet är "". |
| [IsFullPathLink](./isfullpathlink/) | Anger om fullständig sökvägslänk ska användas i sheet00x.htm, filelist.xml och tabstrip.htm. Standardvärdet är falskt. |
| [SetIsFullPathLink](./setisfullpathlink/) | Anger om fullständig sökvägslänk ska användas i sheet00x.htm, filelist.xml och tabstrip.htm. Standardvärdet är falskt. |
| [GetExportWorksheetCSSSeparately](./getexportworksheetcssseparately/) | Anger om arbetsblads‑CSS ska exporteras separat. Standardvärdet är falskt. |
| [SetExportWorksheetCSSSeparately](./setexportworksheetcssseparately/) | Anger om arbetsblads‑CSS ska exporteras separat. Standardvärdet är falskt. |
| [GetExportSimilarBorderStyle](./getexportsimilarborderstyle/) | Anger om liknande kantstil ska exporteras när kantstilen inte stöds av webbläsare. Om du vill importera HTML‑ eller MHT‑filen till Excel, behåll standardvärdet. Standardvärdet är falskt. |
| [SetExportSimilarBorderStyle](./setexportsimilarborderstyle/) | Anger om liknande kantstil ska exporteras när kantstilen inte stöds av webbläsare. Om du vill importera HTML‑ eller MHT‑filen till Excel, behåll standardvärdet. Standardvärdet är falskt. |
| [GetMergeEmptyTdType](./getmergeemptytdtype/) | Alternativet för att slå ihop intilliggande tomma celler (tomma td‑element). Standardvärdet är MergeEmptyTdType.Default. |
| [SetMergeEmptyTdType](./setmergeemptytdtype/) | Alternativet för att slå ihop intilliggande tomma celler (tomma td‑element). Standardvärdet är MergeEmptyTdType.Default. |
| [GetExportCellCoordinate](./getexportcellcoordinate/) | Anger om Excel‑koordinater för icke‑tomma celler ska exporteras när filen sparas som HTML. Standardvärdet är falskt. Om du vill importera den genererade HTML‑filen till Excel, behåll standardvärdet. |
| [SetExportCellCoordinate](./setexportcellcoordinate/) | Anger om Excel‑koordinater för icke‑tomma celler ska exporteras när filen sparas som HTML. Standardvärdet är falskt. Om du vill importera den genererade HTML‑filen till Excel, behåll standardvärdet. |
| [GetExportExtraHeadings](./getexportextraheadings/) | Anger om extra rubriker ska exporteras när textlängden är längre än den maximala visningskolumnen. Standardvärdet är falskt. Om du vill importera HTML‑filen till Excel, behåll standardvärdet. |
| [SetExportExtraHeadings](./setexportextraheadings/) | Anger om extra rubriker ska exporteras när textlängden är längre än den maximala visningskolumnen. Standardvärdet är falskt. Om du vill importera HTML‑filen till Excel, behåll standardvärdet. |
| [GetExportRowColumnHeadings](./getexportrowcolumnheadings/) | Anger om bladets rad- och kolumnrubriker ska exporteras när de sparas som HTML‑filer. |
| [SetExportRowColumnHeadings](./setexportrowcolumnheadings/) | Anger om bladets rad- och kolumnrubriker ska exporteras när de sparas som HTML‑filer. |
| [GetExportFormula](./getexportformula/) | Anger om formler ska exporteras när filen sparas som HTML. Standardvärdet är sant. Om du vill importera den genererade HTML‑filen till Excel, behåll standardvärdet. |
| [SetExportFormula](./setexportformula/) | Anger om formler ska exporteras när filen sparas som HTML. Standardvärdet är sant. Om du vill importera den genererade HTML‑filen till Excel, behåll standardvärdet. |
| [GetAddTooltipText](./getaddtooltiptext/) | Anger om verktygstips ska läggas till när data inte kan visas helt. Standardvärdet är falskt. |
| [SetAddTooltipText](./setaddtooltiptext/) | Anger om verktygstips ska läggas till när data inte kan visas helt. Standardvärdet är falskt. |
| [GetExportGridLines](./getexportgridlines/) | Anger om rutnätslinjer ska exporteras. Standardvärdet är falskt. |
| [SetExportGridLines](./setexportgridlines/) | Anger om rutnätslinjer ska exporteras. Standardvärdet är falskt. |
| [GetExportBogusRowData](./getexportbogusrowdata/) | Anger om falsk data i sista raden ska exporteras. Standardvärdet är sant. Om du vill importera HTML‑ eller MHT‑filen till Excel, behåll standardvärdet. |
| [SetExportBogusRowData](./setexportbogusrowdata/) | Anger om falsk data i sista raden ska exporteras. Standardvärdet är sant. Om du vill importera HTML‑ eller MHT‑filen till Excel, behåll standardvärdet. |
| [GetExcludeUnusedStyles](./getexcludeunusedstyles/) | Anger om oanvända stilar ska uteslutas. För de genererade HTML‑filerna kan uteslutning av oanvända stilar göra filstorleken mindre utan att påverka den visuella effekten. Så standardvärdet för denna egenskap är sant. Om användaren behöver behålla alla stilar i arbetsboken för den genererade HTML‑filen (t.ex. i scenariot där arbetsboken senare ska återställas från den genererade HTML‑filen), sätt egenskapen till falskt. |
| [SetExcludeUnusedStyles](./setexcludeunusedstyles/) | Anger om oanvända stilar ska uteslutas. För de genererade HTML‑filerna kan uteslutning av oanvända stilar göra filstorleken mindre utan att påverka den visuella effekten. Så standardvärdet för denna egenskap är sant. Om användaren behöver behålla alla stilar i arbetsboken för den genererade HTML‑filen (t.ex. i scenariot där arbetsboken senare ska återställas från den genererade HTML‑filen), sätt egenskapen till falskt. |
| [GetExportDocumentProperties](./getexportdocumentproperties/) | Anger om dokumentegenskaper ska exporteras. Standardvärdet är sant. Om du vill importera HTML‑ eller MHT‑filen till Excel, behåll standardvärdet. |
| [SetExportDocumentProperties](./setexportdocumentproperties/) | Anger om dokumentegenskaper ska exporteras. Standardvärdet är sant. Om du vill importera HTML‑ eller MHT‑filen till Excel, behåll standardvärdet. |
| [GetExportWorksheetProperties](./getexportworksheetproperties/) | Anger om arbetsblads‑egenskaper ska exporteras. Standardvärdet är sant. Om du vill importera HTML‑ eller MHT‑filen till Excel, behåll standardvärdet. |
| [SetExportWorksheetProperties](./setexportworksheetproperties/) | Anger om arbetsblads‑egenskaper ska exporteras. Standardvärdet är sant. Om du vill importera HTML‑ eller MHT‑filen till Excel, behåll standardvärdet. |
| [GetExportWorkbookProperties](./getexportworkbookproperties/) | Anger om arbetsboks‑egenskaper ska exporteras. Standardvärdet är sant. Om du vill importera HTML‑ eller MHT‑filen till Excel, behåll standardvärdet. |
| [SetExportWorkbookProperties](./setexportworkbookproperties/) | Anger om arbetsboks‑egenskaper ska exporteras. Standardvärdet är sant. Om du vill importera HTML‑ eller MHT‑filen till Excel, behåll standardvärdet. |
| [GetExportFrameScriptsAndProperties](./getexportframescriptsandproperties/) | Anger om ram‑skript och dokumentegenskaper exporteras. Standardvärdet är true. Om du vill importera html‑ eller mht‑filen till Excel, behåll standardvärdet. |
| [SetExportFrameScriptsAndProperties](./setexportframescriptsandproperties/) | Anger om ram‑skript och dokumentegenskaper exporteras. Standardvärdet är true. Om du vill importera html‑ eller mht‑filen till Excel, behåll standardvärdet. |
| [GetExportDataOptions](./getexportdataoptions/) | Anger regeln för export av html‑fildata. Standardvärdet är All. |
| [SetExportDataOptions](./setexportdataoptions/) | Anger regeln för export av html‑fildata. Standardvärdet är All. |
| [GetLinkTargetType](./getlinktargettype/) | Anger typen av mål‑attribut i <c>&lt;a&gt;</c>-länken. Standardvärdet är HtmlLinkTargetType.Parent. |
| [SetLinkTargetType](./setlinktargettype/) | Anger typen av mål‑attribut i <c>&lt;a&gt;</c>-länken. Standardvärdet är HtmlLinkTargetType.Parent. |
| [IsIECompatible](./isiecompatible/) | Anger om den genererade HTML‑koden är kompatibel med IE‑webbläsaren. Standardvärdet är false. |
| [SetIsIECompatible](./setisiecompatible/) | Anger om den genererade HTML‑koden är kompatibel med IE‑webbläsaren. Standardvärdet är false. |
| [GetFormatDataIgnoreColumnWidth](./getformatdataignorecolumnwidth/) | Anger om hela den formaterade celldata ska visas när den överskrider kolumnen. Om true ignoreras kolumnbredden och hela cellens data exporteras. Om false exporteras data på samma sätt som i Excel. Standardvärdet är false. |
| [SetFormatDataIgnoreColumnWidth](./setformatdataignorecolumnwidth/) | Anger om hela den formaterade celldata ska visas när den överskrider kolumnen. Om true ignoreras kolumnbredden och hela cellens data exporteras. Om false exporteras data på samma sätt som i Excel. Standardvärdet är false. |
| [GetCalculateFormula](./getcalculateformula/) | Anger om formler ska beräknas innan HTML‑filen sparas. |
| [SetCalculateFormula](./setcalculateformula/) | Anger om formler ska beräknas innan HTML‑filen sparas. |
| [IsJsBrowserCompatible](./isjsbrowsercompatible/) | Anger om JavaScript är kompatibel med webbläsare som inte stöder JavaScript. Standardvärdet är true. |
| [SetIsJsBrowserCompatible](./setisjsbrowsercompatible/) | Anger om JavaScript är kompatibel med webbläsare som inte stöder JavaScript. Standardvärdet är true. |
| [IsMobileCompatible](./ismobilecompatible/) | Anger om den genererade HTML‑koden är kompatibel med mobila enheter. Standardvärdet är false. |
| [SetIsMobileCompatible](./setismobilecompatible/) | Anger om den genererade HTML‑koden är kompatibel med mobila enheter. Standardvärdet är false. |
| [GetCssStyles](./getcssstyles/) | Hämtar eller anger ytterligare CSS‑stilar för formateraren. Fungerar endast när SaveAsSingleFile är True. |
| [SetCssStyles](./setcssstyles/) | Hämtar eller anger ytterligare CSS‑stilar för formateraren. Fungerar endast när SaveAsSingleFile är True. |
| [GetHideOverflowWrappedText](./gethideoverflowwrappedtext/) | Anger om överskjutande text ska döljas när cellformatet är inställt på radbrytning. Standardvärdet är false. |
| [SetHideOverflowWrappedText](./sethideoverflowwrappedtext/) | Anger om överskjutande text ska döljas när cellformatet är inställt på radbrytning. Standardvärdet är false. |
| [IsBorderCollapsed](./isbordercollapsed/) | Anger om tabellramarna är sammanslagna. Standardvärdet är true. |
| [SetIsBorderCollapsed](./setisbordercollapsed/) | Anger om tabellramarna är sammanslagna. Standardvärdet är true. |
| [GetEncodeEntityAsCode](./getencodeentityascode/) | Anger om HTML‑teckenentiteter ersätts med decimalkod (t.ex. "&amp;nbsp;" ersätts med "&amp;#160;"). Standardvärdet är false. |
| [SetEncodeEntityAsCode](./setencodeentityascode/) | Anger om HTML‑teckenentiteter ersätts med decimalkod (t.ex. "&amp;nbsp;" ersätts med "&amp;#160;"). Standardvärdet är false. |
| [GetOfficeMathOutputMode](./getofficemathoutputmode/) | Anger hur OfficeMath‑objekt exporteras till HTML. Standardvärdet är Image. |
| [SetOfficeMathOutputMode](./setofficemathoutputmode/) | Anger hur OfficeMath‑objekt exporteras till HTML. Standardvärdet är Image. |
| [GetCellNameAttribute](./getcellnameattribute/) | Anger attributet som specificerar CellName att skrivas (t.ex. om värdet är "id" blir utskriften för cell "A1": &lt;td id='A1'&gt;). Standardvärdet är null. |
| [SetCellNameAttribute](./setcellnameattribute/) | Anger attributet som specificerar CellName att skrivas (t.ex. om värdet är "id" blir utskriften för cell "A1": &lt;td id='A1'&gt;). Standardvärdet är null. |
| [GetDisableCss](./getdisablecss/) | Anger om endast inline‑stilar ska tillämpas, utan att förlita sig på CSS. Standardvärdet är false. |
| [SetDisableCss](./setdisablecss/) | Anger om endast inline‑stilar ska tillämpas, utan att förlita sig på CSS. Standardvärdet är false. |
| [GetEnableCssCustomProperties](./getenablecsscustomproperties/) | Optimera HTML‑utdata genom att använda anpassade CSS‑egenskaper. Till exempel, när en base64‑bild förekommer flera gånger, krävs bilddata endast sparas en gång med en anpassad egenskap, vilket förbättrar prestandan för den resulterande HTML‑koden. Standardvärdet är false. |
| [SetEnableCssCustomProperties](./setenablecsscustomproperties/) | Optimera HTML‑utdata genom att använda anpassade CSS‑egenskaper. Till exempel, när en base64‑bild förekommer flera gånger, krävs bilddata endast sparas en gång med en anpassad egenskap, vilket förbättrar prestandan för den resulterande HTML‑koden. Standardvärdet är false. |
| [GetHtmlVersion](./gethtmlversion/) | Anger vilken version av HTML‑standarden som ska användas vid sparande av HTML‑formatet. Standardvärdet är HtmlVersion.Default. |
| [SetHtmlVersion](./sethtmlversion/) | Anger vilken version av HTML‑standarden som ska användas vid sparande av HTML‑formatet. Standardvärdet är HtmlVersion.Default. |
| [GetSheetSet](./getsheetset/) | Hämtar eller anger bladen som ska renderas. Standard är alla synliga blad i arbetsboken: Aspose.Cells.Rendering.SheetSet.Visible. |
| [SetSheetSet](./setsheetset/) | Hämtar eller anger bladen som ska renderas. Standard är alla synliga blad i arbetsboken: Aspose.Cells.Rendering.SheetSet.Visible. |
| [GetLayoutMode](./getlayoutmode/) | Hämtar eller anger layoutläget vid sparande till HTML. Standardvärdet är HtmlLayoutMode.Normal. |
| [SetLayoutMode](./setlayoutmode/) | Hämtar eller anger layoutläget vid sparande till HTML. Standardvärdet är HtmlLayoutMode.Normal. |
| [GetEmbeddedFontType](./getembeddedfonttype/) | Hämtar eller anger typen av inbäddad teckensnittsfil i HTML‑filen. Standardvärdet är HtmlEmbeddedFontType.None, vilket innebär att ingen teckensnitt inbäddas i HTML. |
| [SetEmbeddedFontType](./setembeddedfonttype/) | Hämtar eller anger typen av inbäddad teckensnittsfil i HTML‑filen. Standardvärdet är HtmlEmbeddedFontType.None, vilket innebär att ingen teckensnitt inbäddas i HTML. |
| [GetExportNamedRangeAnchors](./getexportnamedrangeanchors/) | Anger om ankarelement för namngivna områden ska exporteras vid sparande som HTML. Standardvärdet är true. |
| [SetExportNamedRangeAnchors](./setexportnamedrangeanchors/) | Anger om ankarelement för namngivna områden ska exporteras vid sparande som HTML. Standardvärdet är true. |
| [GetDataBarRenderMode](./getdatabarrendermode/) | Representerar läget för hur DataBar renderas vid konvertering av Excel‑filer till HTML‑filer. Standardvärdet är DataBarRenderMode.BackgroundColor. |
| [SetDataBarRenderMode](./setdatabarrendermode/) | Representerar läget för hur DataBar renderas vid konvertering av Excel‑filer till HTML‑filer. Standardvärdet är DataBarRenderMode.BackgroundColor. |
| [GetSpaceMode](./getspacemode/) | Anger hur mellanslag renderas i HTML‑utdata. Detta alternativ tillämpas för närvarande endast på numeriska format (t.ex. bokföringsformat). Standardvärdet är HtmlSpaceMode.Css. |
| [SetSpaceMode](./setspacemode/) | Anger hur mellanslag renderas i HTML‑utdata. Detta alternativ tillämpas för närvarande endast på numeriska format (t.ex. bokföringsformat). Standardvärdet är HtmlSpaceMode.Css. |
| [GetSaveFormat](./getsaveformat/) | Hämtar formatet för sparad fil. |
| [GetClearData](./getcleardata/) | Gör arbetsboken tom efter att filen har sparats. |
| [SetClearData](./setcleardata/) | Gör arbetsboken tom efter att filen har sparats. |
| [GetCachedFileFolder](./getcachedfilefolder/) | Mappen för temporära filer som kan användas som datacache. |
| [SetCachedFileFolder](./setcachedfilefolder/) | Mappen för temporära filer som kan användas som datacache. |
| [GetValidateMergedAreas](./getvalidatemergedareas/) | Anger om sammanslagna celler ska valideras innan filen sparas. |
| [SetValidateMergedAreas](./setvalidatemergedareas/) | Anger om sammanslagna celler ska valideras innan filen sparas. |
| [GetMergeAreas](./getmergeareas/) | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. |
| [SetMergeAreas](./setmergeareas/) | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. |
| [GetCreateDirectory](./getcreatedirectory/) | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. |
| [SetCreateDirectory](./setcreatedirectory/) | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. |
| [GetSortNames](./getsortnames/) | Anger om definierade namn ska sorteras innan filen sparas. |
| [SetSortNames](./setsortnames/) | Anger om definierade namn ska sorteras innan filen sparas. |
| [GetSortExternalNames](./getsortexternalnames/) | Anger om externa definierade namn ska sorteras innan filen sparas. |
| [SetSortExternalNames](./setsortexternalnames/) | Anger om externa definierade namn ska sorteras innan filen sparas. |
| [GetRefreshChartCache](./getrefreshchartcache/) | Anger om den senaste datan för diagrammet ska cachas. |
| [SetRefreshChartCache](./setrefreshchartcache/) | Anger om den senaste datan för diagrammet ska cachas. |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | Om kontroll av begränsningar i Excel-filen när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32K. När du matar in ett värde längre än 32K kommer det att trunkeras. |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | Om kontroll av begränsningar i Excel-filen när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32K. När du matar in ett värde längre än 32K kommer det att trunkeras. |
| [GetUpdateSmartArt](./getupdatesmartart/) | Anger om smart art-inställningarna ska uppdateras. Standardvärdet är false. |
| [SetUpdateSmartArt](./setupdatesmartart/) | Anger om smart art-inställningarna ska uppdateras. Standardvärdet är false. |
| [GetEncryptDocumentProperties](./getencryptdocumentproperties/) | Anger om dokumentegenskaper ska krypteras när du sparar som .xls-fil. Standardvärdet är true. |
| [SetEncryptDocumentProperties](./setencryptdocumentproperties/) | Anger om dokumentegenskaper ska krypteras när du sparar som .xls-fil. Standardvärdet är true. |
