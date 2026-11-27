---
title: "Klass Config"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridJs.Config-klass. Representerar alla statiska inställningar för GridJs"
type: docs
url: /sv/net/aspose.cells.gridjs/config/
---
## Config class

Representerar alla statiska inställningar för GridJs.

```csharp
public class Config
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [Config](config/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| static [AutoFitColumnsOnLoad](../../aspose.cells.gridjs/config/autofitcolumnsonload/) { get; set; } | Anger om kolumnbredder ska automatiskt anpassas vid filinläsning. Standardvärdet är `false`. Varning: Om detta sätts till `true` utförs en automatisk anpassning av alla kolumner efter inläsning, vilket kan ha en märkbar inverkan på prestandan. |
| static [AutoFitRowsHeightOnLoad](../../aspose.cells.gridjs/config/autofitrowsheightonload/) { get; set; } | Anger om radhöjder ska automatiskt anpassas vid filinläsning. Standardvärdet är `false`. Varning: Om detta sätts till `true` utförs en automatisk anpassning av alla rader efter inläsning, vilket kan ha en märkbar inverkan på prestandan. |
| static [AutoOptimizeForLargeCells](../../aspose.cells.gridjs/config/autooptimizeforlargecells/) { get; set; } | Hämtar/Sätter om laddningsprestandan automatiskt ska optimeras för kalkylblad med stora celler. Det kommer att ignorera vissa stilar /kanter för att minska laddningstiden. Standardvärdet är sant. |
| static [BaseRouteName](../../aspose.cells.gridjs/config/baseroutename/) { get; set; } | Hämtar/Anger basruttens namn för GridJs‑controller‑URL. Standardvärdet är "/GridJs2". |
| static [CustomPdfSaveOptions](../../aspose.cells.gridjs/config/custompdfsaveoptions/) { get; set; } | Hämtar/Sätter de anpassade PdfSaveOptions för PDF‑export. Om angivet kommer detta att användas i stället för standardalternativen. Standardvärdet är null. |
| static [EmptySheetMaxCol](../../aspose.cells.gridjs/config/emptysheetmaxcol/) { get; set; } | Hämtar/Sätter standard maximal kolumn för ett tomt kalkylblad. Standardvärdet är 15. |
| static [EmptySheetMaxRow](../../aspose.cells.gridjs/config/emptysheetmaxrow/) { get; set; } | Hämtar/Sätter standard maximal rad för ett tomt kalkylblad. Standardvärdet är 12. |
| static [EnableChartClientRendering](../../aspose.cells.gridjs/config/enablechartclientrendering/) { get; set; } | Hämtar/Anger om klient‑sidans diagramrendering ska aktiveras. Om den är falsk (`false`) kommer GridJs att falla tillbaka till endast servergenererade diagrambilder/‑former. Standardvärdet är `true`. |
| static [FileCacheDirectory](../../aspose.cells.gridjs/config/filecachedirectory/) { get; set; } | Hämtar/Sätter cache‑katalogen för lagring av kalkylbladsfil. Vi måste ange en specifik sökväg innan vi använder GridJs. |
| static [IgnoreEmptyContent](../../aspose.cells.gridjs/config/ignoreemptycontent/) { get; set; } | Hämtar/Sätter om det maximala intervallet som inkluderar data, stil, sammanslagna celler och former ska visas. Om den sista raden eller kolumnen innehåller celler utan värde och formel men med anpassad stil visas inte den raden/kolumnen när detta värde är sant. Standardvärdet är sant. |
| static [IsCollaborative](../../aspose.cells.gridjs/config/iscollaborative/) { get; set; } | Hämtar/Sätter om samarbetsredigering ska stödjas, standard är falskt. |
| static [IslimitShapeOrImage](../../aspose.cells.gridjs/config/islimitshapeorimage/) { get; set; } | Hämtar/Sätter om det totala antalet visade former/bilder i ett kalkylblad ska begränsas, om satt till sant kommer GridJs att begränsa det totala antalet visade former eller bilder i ett kalkylblad till MaxShapeOrImageCount. Standardvärdet är sant. |
| static [IsWasm](../../aspose.cells.gridjs/config/iswasm/) { get; set; } | Hämtar/Anger om GridJs körs i en webbläsar‑WebAssembly‑värd istället för en serverprocess. När den är `true` används ingen FileCacheDirectory / disk / interrupt‑thread‑sökväg och filcachen måste komma från GridJsOptions.CacheImp. GridJsOptions.IsWasm sätter detta när GridJs‑tjänsten konstrueras, så en Aspose.Cells.GridJs.dll kan betjäna båda värdarna. Standardvärdet är `false`. |
| static [JsonCache](../../aspose.cells.gridjs/config/jsoncache/) { get; set; } | Hämtar/Sätter JSON‑cache‑konfigurationsalternativ. Styr både minnes‑ (L1) och disk‑ (L2) cachebeteende för genererad arbetsbok‑JSON. |
| static [LazyLoading](../../aspose.cells.gridjs/config/lazyloading/) { get; set; } | Hämtar/Sätter om endast det aktiva kalkylbladet ska laddas, standard är falskt. |
| static [MaxPdfSaveSeconds](../../aspose.cells.gridjs/config/maxpdfsaveseconds/) { get; set; } | Hämtar/Sätter maximalt antal sekunder för timeout vid sparande till PDF. Standardvärdet är 10. |
| static [MaxShapeOrImageCount](../../aspose.cells.gridjs/config/maxshapeorimagecount/) { get; set; } | Hämtar/Sätter det totala antalet visade former eller bilder i det aktiva bladet, gäller när IslimitShapeOrImage=sant. Standardvärdet är 100. |
| static [MaxShapeOrImageWidthOrHeight](../../aspose.cells.gridjs/config/maxshapeorimagewidthorheight/) { get; set; } | Hämtar/Sätter maximal bredd eller höjd för en form eller bild, GridJs ignorerar former eller bilder med bredd eller höjd som överstiger detta, gäller när IslimitShapeOrImage=sant. Standardvärdet är 10000. |
| static [MaxTotalShapeOrImageCount](../../aspose.cells.gridjs/config/maxtotalshapeorimagecount/) { get; set; } | Hämtar/Sätter det totala antalet visade former eller bilder i arbetsboken, gäller när IslimitShapeOrImage=sant. Standardvärdet är 300. |
| static [MessageTopic](../../aspose.cells.gridjs/config/messagetopic/) { get; set; } | Hämtar/Anger websocket‑destinationerna med prefix \"/topic\". standardvärdet är \"/topic/opr\". används endast i samarbetsläge. |
| static [PictureCacheDirectory](../../aspose.cells.gridjs/config/picturecachedirectory/) { get; set; } | Hämtar/Anger cache‑katalogen för bilder. (detta träder i kraft när GridJsWorkbook.CacheImp är null) standard‑sökvägen blir \"_piccache\" i FileCacheDirectory. |
| static [SameImageDetecting](../../aspose.cells.gridjs/config/sameimagedetecting/) { get; set; } | Hämtar/Anger om man ska kontrollera om bilder har samma källa, standard är true, standardvärdet är true. |
| static [SaveHtmlAsZip](../../aspose.cells.gridjs/config/savehtmlaszip/) { get; set; } | Hämtar/Anger om HTML‑filen ska sparas som zip‑arkiv, standard är false. |
| static [ShowChartSheet](../../aspose.cells.gridjs/config/showchartsheet/) { get; set; } | Hämtar/Anger om diagram‑arbetsbladet ska visas. standardvärdet är false. |
| static [SkipInvisibleShapes](../../aspose.cells.gridjs/config/skipinvisibleshapes/) { get; set; } | Hämtar/Anger om former som är osynliga för UI ska hoppas över, standardvärdet är true. |
| static [UsePrintArea](../../aspose.cells.gridjs/config/useprintarea/) { get; set; } | Hämtar/Anger om PageSetup.PrintArea ska användas för UI‑visningsområdet när kalkylbladet har PageSetup‑inställning för PrintArea. standardvärdet är false. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| static [SetFontFolder](../../aspose.cells.gridjs/config/setfontfolder/)(string, bool) | Anger teckensnittsmappen |
| static [SetFontFolders](../../aspose.cells.gridjs/config/setfontfolders/)(string[], bool) | Anger teckensnittsmapparna |

## Fält

| Namn | Beskrivning |
| --- | --- |
| static [RedactionUseClientGenerateId](../../aspose.cells.gridjs/config/redactionuseclientgenerateid/) | Indikerar om klienten ska generera ID istället för det faktiska form‑ID:t i redigeringsrelaterade operationer. |

### Se även

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


