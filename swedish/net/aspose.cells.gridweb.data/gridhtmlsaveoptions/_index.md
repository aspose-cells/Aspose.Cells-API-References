---
title: "Klass GridHtmlSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridWeb.Data.GridHtmlSaveOptions-klass. Representerar alternativen för att spara html‑fil."
type: docs
url: /sv/net/aspose.cells.gridweb.data/gridhtmlsaveoptions/
---
## GridHtmlSaveOptions class

Representerar alternativen för att spara HTML-fil.

```csharp
public class GridHtmlSaveOptions : GridSaveOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [GridHtmlSaveOptions](gridhtmlsaveoptions/#constructor)() | Skapar alternativ för att spara en html‑fil. |
| [GridHtmlSaveOptions](gridhtmlsaveoptions/#constructor_1)(GridSaveFormat) | Skapar alternativ för att spara en htm‑fil. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AttachedFilesDirectory](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesdirectory/) { get; set; } | Den katalog som de bifogade filerna kommer att sparas i. Endast för att spara till html‑ström. |
| [AttachedFilesUrlPrefix](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesurlprefix/) { get; set; } | Ange Url‑prefixet för bifogade filer, såsom bild i html‑filen. Endast för att spara till html‑ström. |
| [CachedFileFolder](../../aspose.cells.gridweb.data/gridsaveoptions/cachedfilefolder/) { get; set; } | Den cachade filmappen används för att lagra viss stor data.(ärvd från [`GridSaveOptions`](../gridsaveoptions/).) |
| [ClearData](../../aspose.cells.gridweb.data/gridsaveoptions/cleardata/) { get; set; } | Gör arbetsboken tom efter att filen har sparats.(ärvd från [`GridSaveOptions`](../gridsaveoptions/).) |
| [CreateDirectory](../../aspose.cells.gridweb.data/gridsaveoptions/createdirectory/) { get; set; } | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas.(ärvd från [`GridSaveOptions`](../gridsaveoptions/).) |
| [DefaultFontName](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/defaultfontname/) { get; set; } | Ange standardteckensnittets namn för export av html, standardteckensnittet används när stilens teckensnitt inte finns. Om denna egenskap är null kommer Aspose.Cells att använda ett universellt teckensnitt som har samma familj som originalteckensnittet, standardvärdet är null. |
| [Encoding](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/encoding/) { get; set; } | Om inte angivet, använd Encoding.UTF8 som standardkodningstyp. |
| [ExportActiveWorksheetOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportactiveworksheetonly/) { get; set; } | Anger om hela arbetsboken exporteras till en html‑fil. |
| [ExportArea](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportarea/) { get; set; } | Hämtar eller anger det exporterande CellArea för det aktuella aktiva kalkylbladet. Om du anger detta attribut kommer utskriftsområdet för det aktuella aktiva kalkylbladet att utelämnas. Endast det angivna området kommer att exporteras när filen sparas till html. |
| [ExportGridLines](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportgridlines/) { get; set; } | Anger om rutnät ska exporteras. Standardvärdet är false. |
| [ExportHeadings](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportheadings/) { get; set; } | Anger om rubriker ska exporteras när filen sparas till html. Standardvärdet är false. Om du vill importera html‑filen till Excel, behåll standardvärdet. |
| [ExportHiddenWorksheet](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exporthiddenworksheet/) { get; set; } | Anger om dolt kalkylbladsinnehåll ska exporteras. Standardvärdet är true. |
| [ExportImagesAsBase64](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportimagesasbase64/) { get; set; } | Anger om bilder sparas i Base64-format till HTML, MHTML eller EPUB. |
| [ExportPrintAreaOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportprintareaonly/) { get; set; } | Anger om endast utskriftsområdet ska exporteras till html-fil. Standardvärdet är false. |
| [ExportSingleTab](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportsingletab/) { get; set; } | Anger om den enda fliken ska exporteras när filen bara har ett kalkylblad. Standardvärdet är false. |
| [IsExportComments](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isexportcomments/) { get; set; } | Anger om kommentarer ska exporteras när filen sparas i HTML, standardvärdet är false. |
| [IsFullPathLink](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isfullpathlink/) { get; set; } | Anger om fullständig sökväg ska användas i länkar i sheet00x.htm, filelist.xml och tabstrip.htm. Standardvärdet är false. |
| [MergeAreas](../../aspose.cells.gridweb.data/gridsaveoptions/mergeareas/) { get; set; } | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas.(ärvd från [`GridSaveOptions`](../gridsaveoptions/).) |
| [PageTitle](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/pagetitle/) { get; set; } | Titeln på HTML-sidan. Endast för att spara till HTML-ström. |
| [ParseHtmlTagInCell](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/parsehtmltagincell/) { get; set; } | Analysera html‑tagg i cell, som , som cellvärde, eller som html‑tagg, standard är true |
| [PresentationPreference](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/presentationpreference/) { get; set; } | Anger om html‑ eller mht‑fil är presentationspreferens. Standardvärdet är false. Om du vill ha en vackrare presentation, sätt värdet till true. |
| [RefreshChartCache](../../aspose.cells.gridweb.data/gridsaveoptions/refreshchartcache/) { get; set; } | Anger om diagrammets cachedata ska uppdateras (ärvd från [`GridSaveOptions`](../gridsaveoptions/).) |
| [SaveFormat](../../aspose.cells.gridweb.data/gridsaveoptions/saveformat/) { get; } | Hämtar filformatet för sparning.(ärvd från [`GridSaveOptions`](../gridsaveoptions/).) |
| [SortNames](../../aspose.cells.gridweb.data/gridsaveoptions/sortnames/) { get; set; } | Anger om definierade namn ska sorteras innan filen sparas.(ärvd från [`GridSaveOptions`](../gridsaveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells.gridweb.data/gridsaveoptions/validatemergedareas/) { get; set; } | Anger om sammanslagna celler ska valideras innan filen sparas.(ärvd från [`GridSaveOptions`](../gridsaveoptions/).) |

### Se även

* class [GridSaveOptions](../gridsaveoptions/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


