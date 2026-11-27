---
title: "Klass GridJsOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridJs.GridJsOptions klass. Representerar alla laddningsalternativ för GridJs"
type: docs
url: /sv/net/aspose.cells.gridjs/gridjsoptions/
---
## GridJsOptions class

Representerar alla laddningsalternativ för GridJs

```csharp
public class GridJsOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [GridJsOptions](gridjsoptions/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AutoFitColumnsOnLoad](../../aspose.cells.gridjs/gridjsoptions/autofitcolumnsonload/) { get; set; } | Anger om kolumnbredden ska autofitas vid inläsning av filen, standardvärdet är falskt. |
| [AutoFitRowsHeightOnLoad](../../aspose.cells.gridjs/gridjsoptions/autofitrowsheightonload/) { get; set; } | Anger om radhöjden ska autofitas vid inläsning av filen, standardvärdet är falskt. |
| [AutoOptimizeForLargeCells](../../aspose.cells.gridjs/gridjsoptions/autooptimizeforlargecells/) { get; set; } | Hämtar/Sätter om laddningsprestandan automatiskt ska optimeras för kalkylblad med stora celler. Det kommer att ignorera vissa stilar /kanter för att minska laddningstiden. Standardvärdet är sant. |
| [BaseRouteName](../../aspose.cells.gridjs/gridjsoptions/baseroutename/) { get; set; } | Hämtar/Sätter basnamnet för route‑URL för GridJs‑kontrollen. Standard är GridJs2 |
| [CustomPdfSaveOptions](../../aspose.cells.gridjs/gridjsoptions/custompdfsaveoptions/) { get; set; } | Hämtar/Sätter de anpassade PdfSaveOptions för PDF‑export. Om angivet kommer detta att användas i stället för standardalternativen. Standardvärdet är null. |
| [EmptySheetMaxCol](../../aspose.cells.gridjs/gridjsoptions/emptysheetmaxcol/) { get; set; } | Hämtar/Sätter standard maximal kolumn för ett tomt kalkylblad. Standardvärdet är 15. |
| [EmptySheetMaxRow](../../aspose.cells.gridjs/gridjsoptions/emptysheetmaxrow/) { get; set; } | Hämtar/Sätter standard maximal rad för ett tomt kalkylblad. Standardvärdet är 12. |
| [EnableChartClientRendering](../../aspose.cells.gridjs/gridjsoptions/enablechartclientrendering/) { get; set; } | Hämtar/Sätter om klient‑sidans diagramrendering ska aktiveras. Om satt till falskt kommer GridJs endast att generera diagrambilder/‑former och kräver inte klient‑sidans rendering. Standardvärdet är sant. |
| [FileCacheDirectory](../../aspose.cells.gridjs/gridjsoptions/filecachedirectory/) { get; set; } | Hämtar/Sätter cache‑katalogen för lagring av kalkylbladsfil. Vi måste ange en specifik sökväg innan vi använder GridJs. |
| [FontFolders](../../aspose.cells.gridjs/gridjsoptions/fontfolders/) { get; set; } | Hämtar/Sätter teckensnittsmapparna för teckensnitt i de renderade bilderna/‑formerna |
| [IgnoreEmptyContent](../../aspose.cells.gridjs/gridjsoptions/ignoreemptycontent/) { get; set; } | Hämtar/Sätter om det maximala intervallet som inkluderar data, stil, sammanslagna celler och former ska visas. Om den sista raden eller kolumnen innehåller celler utan värde och formel men med anpassad stil visas inte den raden/kolumnen när detta värde är sant. Standardvärdet är sant. |
| [IsCollaborative](../../aspose.cells.gridjs/gridjsoptions/iscollaborative/) { get; set; } | Hämtar/Sätter om samarbetsredigering ska stödjas, standard är falskt. |
| [IslimitShapeOrImage](../../aspose.cells.gridjs/gridjsoptions/islimitshapeorimage/) { get; set; } | Hämtar/Sätter om det totala antalet visade former/bilder i ett kalkylblad ska begränsas, om satt till sant kommer GridJs att begränsa det totala antalet visade former eller bilder i ett kalkylblad till MaxShapeOrImageCount. Standardvärdet är sant. |
| [IsWasm](../../aspose.cells.gridjs/gridjsoptions/iswasm/) { get; set; } | Hämtar/Sätter om GridJs körs i en webbläsar‑WebAssembly‑värd i stället för en serverprocess. När sant används ingen FileCacheDirectory / disk / avbrotts‑trådsökväg, och filcachen måste komma från CacheImp, eftersom en webbläsarvärd saknar lokal disk. Den väljer kodvägar vid körning, så en Aspose.Cells.GridJs.dll betjänar båda värdarna. Standardvärdet är falskt. |
| [JsonCache](../../aspose.cells.gridjs/gridjsoptions/jsoncache/) { get; set; } | Hämtar/Sätter JSON‑cache‑konfigurationsalternativ. Styr både minnes‑ (L1) och disk‑ (L2) cachebeteende för genererad arbetsbok‑JSON. |
| [LazyLoading](../../aspose.cells.gridjs/gridjsoptions/lazyloading/) { get; set; } | Hämtar/Sätter om endast det aktiva kalkylbladet ska laddas, standard är falskt. |
| [MaxPdfSaveSeconds](../../aspose.cells.gridjs/gridjsoptions/maxpdfsaveseconds/) { get; set; } | Hämtar/Sätter maximalt antal sekunder för timeout vid sparande till PDF. Standardvärdet är 10. |
| [MaxShapeOrImageCount](../../aspose.cells.gridjs/gridjsoptions/maxshapeorimagecount/) { get; set; } | Hämtar/Sätter det totala antalet visade former eller bilder i det aktiva bladet, gäller när IslimitShapeOrImage=sant. Standardvärdet är 100. |
| [MaxShapeOrImageWidthOrHeight](../../aspose.cells.gridjs/gridjsoptions/maxshapeorimagewidthorheight/) { get; set; } | Hämtar/Sätter maximal bredd eller höjd för en form eller bild, GridJs ignorerar former eller bilder med bredd eller höjd som överstiger detta, gäller när IslimitShapeOrImage=sant. Standardvärdet är 10000. |
| [MaxTotalShapeOrImageCount](../../aspose.cells.gridjs/gridjsoptions/maxtotalshapeorimagecount/) { get; set; } | Hämtar/Sätter det totala antalet visade former eller bilder i arbetsboken, gäller när IslimitShapeOrImage=sant. Standardvärdet är 300. |
| [MessageTopic](../../aspose.cells.gridjs/gridjsoptions/messagetopic/) { get; set; } | Hämtar/Anger websocket‑destinationerna med prefix \"/topic\". standardvärdet är \"/topic/opr\". används endast i samarbetsläge. |
| [PictureCacheDirectory](../../aspose.cells.gridjs/gridjsoptions/picturecachedirectory/) { get; set; } | Hämtar/Anger cache‑katalogen för bilder. (detta träder i kraft när GridJsWorkbook.CacheImp är null) standard‑sökvägen blir \"_piccache\" i FileCacheDirectory. |
| [SameImageDetecting](../../aspose.cells.gridjs/gridjsoptions/sameimagedetecting/) { get; set; } | Hämtar/Anger om man ska kontrollera om bilder har samma källa, standard är true, standardvärdet är true. |
| [SaveHtmlAsZip](../../aspose.cells.gridjs/gridjsoptions/savehtmlaszip/) { get; set; } | Hämtar/Anger om HTML‑filen ska sparas som zip‑arkiv, standard är false. |
| [ShowChartSheet](../../aspose.cells.gridjs/gridjsoptions/showchartsheet/) { get; set; } | Hämtar/Anger om diagram‑arbetsbladet ska visas. standardvärdet är false. |
| [SkipInvisibleShapes](../../aspose.cells.gridjs/gridjsoptions/skipinvisibleshapes/) { get; set; } | Hämtar/Anger om former som är osynliga för UI ska hoppas över, standardvärdet är true. |
| [UsePrintArea](../../aspose.cells.gridjs/gridjsoptions/useprintarea/) { get; set; } | Hämtar/Anger om PageSetup.PrintArea ska användas för UI‑visningsområdet när kalkylbladet har PageSetup‑inställning för PrintArea. standardvärdet är false. |

## Fält

| Namn | Beskrivning |
| --- | --- |
| [CacheImp](../../aspose.cells.gridjs/gridjsoptions/cacheimp/) | Anpassad implementation för cache‑lagring. Om du vill lagra cache i ström‑format måste du ange och implementera den. En WebAssembly‑värd (IsWasm = true) måste sätta den, eftersom det inte finns någon lokal disk för standard‑filcachen. |
| [RedactionUseClientGenerateId](../../aspose.cells.gridjs/gridjsoptions/redactionuseclientgenerateid/) | Indikerar om klienten ska generera ID istället för det faktiska form‑ID:t i redigeringsrelaterade operationer. |

### Se även

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


