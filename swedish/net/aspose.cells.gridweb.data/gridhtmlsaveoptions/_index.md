---
title: GridHtmlSaveOptions
second_title: Aspose.Cells för .NET API-referens
description: Representerar alternativen för att spara html-fil.
type: docs
weight: 250
url: /sv/net/aspose.cells.gridweb.data/gridhtmlsaveoptions/
---
## GridHtmlSaveOptions class

Representerar alternativen för att spara html-fil.

```csharp
public class GridHtmlSaveOptions : GridSaveOptions
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [GridHtmlSaveOptions](gridhtmlsaveoptions#constructor)() | Skapar alternativ för att spara html-fil. |
| [GridHtmlSaveOptions](gridhtmlsaveoptions#constructor_1)(GridSaveFormat) | Skapar alternativ för att spara htm-fil. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [AttachedFilesDirectory](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesdirectory) { get; set; } | Mappen som de bifogade filerna kommer att sparas i. Endast för att spara till html-ström. |
| [AttachedFilesUrlPrefix](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesurlprefix) { get; set; } | Ange URL-prefixet för bifogade filer såsom bild i html-filen. Endast för att spara till html-ström. |
| [CachedFileFolder](../../aspose.cells.gridweb.data/gridsaveoptions/cachedfilefolder) { get; set; } | Den cachade filmappen används för att lagra en del stora data. |
| [ClearData](../../aspose.cells.gridweb.data/gridsaveoptions/cleardata) { get; set; } | Gör arbetsboken tom när du har sparat filen. |
| [CreateDirectory](../../aspose.cells.gridweb.data/gridsaveoptions/createdirectory) { get; set; } | Om true och katalogen inte finns skapas katalogen automatiskt innan filen sparas. |
| [DefaultFontName](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/defaultfontname) { get; set; } | Ange standardteckensnittsnamnet för att exportera html, standardteckensnittet kommer att användas när stilteckensnittet inte finns, Om denna egenskap är null kommer Aspose.Cells att använda universella teckensnitt som har samma familj med det ursprungliga teckensnittet, standardvärdet är null. |
| [Encoding](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/encoding) { get; set; } | Om inte inställt, använd Encoding.UTF8 som standardkodningstyp. |
| [ExportActiveWorksheetOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportactiveworksheetonly) { get; set; } | Indikerar om hela arbetsboken exporteras till html-fil. |
| [ExportArea](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportarea) { get; set; } | Hämtar eller ställer in det exporterande cellområdet för det aktuella aktiva kalkylbladet. Om du ställer in det här attributet kommer utskriftsområdet för det aktuella aktiva kalkylbladet att utelämnas. Endast det angivna området kommer att exporteras när filen sparas till html. |
| [ExportGridLines](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportgridlines) { get; set; } | Indikerar om rutnätslinjerna exporteras. Standardvärdet är false. |
| [ExportHeadings](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportheadings) { get; set; } | Indikerar om rubriker exporteras när filen sparas till html. Standardvärdet är false. Om du vill importera html-filen till Excel, behåll standardvärdet. |
| [ExportHiddenWorksheet](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exporthiddenworksheet) { get; set; } | Indikerar om det dolda kalkylbladets innehåll exporteras. Standardvärdet är sant. |
| [ExportImagesAsBase64](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportimagesasbase64) { get; set; } | Anger om bilder sparas i Base64-format till HTML, MHTML eller EPUB. |
| [ExportPrintAreaOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportprintareaonly) { get; set; } | Indikerar om utskriftsområdet endast exporteras till html-fil. Standardvärdet är false. |
| [ExportSingleTab](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportsingletab) { get; set; } | Anger om den enskilda fliken exporteras när filen bara har ett kalkylblad. Standardvärdet är false. |
| [IsExportComments](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isexportcomments) { get; set; } | Indikerar om kommentarer exporteras när filen sparas till html, standardvärdet är false. |
| [IsFullPathLink](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isfullpathlink) { get; set; } | Indikerar om fullständig sökvägslänk används i sheet00x.htm,filelist.xml och tabstrip.htm. Standardvärdet är false. |
| [MergeAreas](../../aspose.cells.gridweb.data/gridsaveoptions/mergeareas) { get; set; } | Anger om områdena för villkorlig formatering och validering slås samman innan filen sparas. |
| [PageTitle](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/pagetitle) { get; set; } | Titeln på HTML-sidan. Endast för att spara till HTML-ström. |
| [ParseHtmlTagInCell](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/parsehtmltagincell) { get; set; } | Analysera HTML-tagg i cell, som ,som cellvärde,eller som html-tagg,standard är true |
| [PresentationPreference](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/presentationpreference) { get; set; } | Indikerar om html- eller mht-fil är presentationspreferens. Standardvärdet är false. Om du vill få en vackrare presentation, ställ in värdet till true. |
| [RefreshChartCache](../../aspose.cells.gridweb.data/gridsaveoptions/refreshchartcache) { get; set; } | Indikerar om uppdatering av diagramcachedata |
| [SaveFormat](../../aspose.cells.gridweb.data/gridsaveoptions/saveformat) { get; } | Hämtar spara filformatet. |
| [SortNames](../../aspose.cells.gridweb.data/gridsaveoptions/sortnames) { get; set; } | Indikerar om du sorterar definierade namn innan filen sparas. |
| [ValidateMergedAreas](../../aspose.cells.gridweb.data/gridsaveoptions/validatemergedareas) { get; set; } | Anger om validera sammanslagna celler innan filen sparas. |

### Se även

* class [GridSaveOptions](../gridsaveoptions)
* namnutrymme [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* hopsättning [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
