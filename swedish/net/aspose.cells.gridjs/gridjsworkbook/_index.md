---
title: "Klass GridJsWorkbook"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridJs.GridJsWorkbook-klass. Representerar huvudindataklassen för GridJs"
type: docs
url: /sv/net/aspose.cells.gridjs/gridjsworkbook/
---
## GridJsWorkbook class

Representerar huvudindataklassen för GridJs

```csharp
public class GridJsWorkbook
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [GridJsWorkbook](gridjsworkbook/)() | Skapar en ny instans av GridJsWorkbook. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CacheDirectory](../../aspose.cells.gridjs/gridjsworkbook/cachedirectory/) { get; set; } | Hämtar/Anger cache‑katalogen för lagring av kalkylbladsfil. Om detta inte är angivet använder vi den statiska egenskapen från [`FileCacheDirectory`](../config/filecachedirectory/) eller [`CacheImp`](./cacheimp/) . |
| [Settings](../../aspose.cells.gridjs/gridjsworkbook/settings/) { get; set; } | Representerar arbetsbokens inställningar. |
| [WarningCallback](../../aspose.cells.gridjs/gridjsworkbook/warningcallback/) { get; set; } | Hämtar eller anger varnings‑callback för importfil. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [BurnRedactionFile](../../aspose.cells.gridjs/gridjsworkbook/burnredactionfile/)(string, string) | Utför (tillämpa) alla raderingsoperationer i arbetsboken genom att ta bort raderingsformer och deras målformer eller rensa innehållet i målcellintervallet. |
| [CheckInCacheForCollaborative](../../aspose.cells.gridjs/gridjsworkbook/checkincacheforcollaborative/)(string) | Kontrollera om arbetsboksinstansen finns i minnescachen. Denna metod gäller endast för samarbetsläge. |
| [ClearAllJsonCache](../../aspose.cells.gridjs/gridjsworkbook/clearalljsoncache/)() | Rensa all JSON‑cache |
| [ClearJsonCacheForUid](../../aspose.cells.gridjs/gridjsworkbook/clearjsoncacheforuid/)(string) | Rensa JSON‑cache baserat på uid (för scenarier som UpdateCell där endast uid finns) |
| [CopyImageOrShape](../../aspose.cells.gridjs/gridjsworkbook/copyimageorshape/)(string, string) | Kopierar bild eller form. |
| [Dispose](../../aspose.cells.gridjs/gridjsworkbook/dispose/)() | Utför applikationsdefinierade uppgifter som är kopplade till att frigöra, släppa eller återställa ohanterade resurser. |
| [ErrorJson](../../aspose.cells.gridjs/gridjsworkbook/errorjson/)(string) | Hämtar felmeddelandet som en sträng i JSON‑format. |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson/#exporttojson)() | Hämtar JSON‑sträng från minnesdata, standardfilnamnet i JSON är: book1. |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson/#exporttojson_1)(string) | Hämtar JSON‑sträng från minnesdata, ange utdatafilnamnet i JSON. |
| [ExportToJsonStringBuilder](../../aspose.cells.gridjs/gridjsworkbook/exporttojsonstringbuilder/)(string, string) | Hämtar JSON‑sträng från minnesdata, ange utdatafilnamnet i JSON. |
| [GetJsonByUid](../../aspose.cells.gridjs/gridjsworkbook/getjsonbyuid/)(string, string) | Hämtar JSON‑strängen för filen från cachen med det angivna unika ID:t, och sätter utdatafilnamnet i JSON‑en. |
| [GetOle](../../aspose.cells.gridjs/gridjsworkbook/getole/)(string, string, int, out string) | Hämtar byte‑array‑data för det inbäddade OLE‑objektet. |
| [GetSheetJsonWithCache](../../aspose.cells.gridjs/gridjsworkbook/getsheetjsonwithcache/)(string, string, string) | Hämtar JSON för angivet blad (med cache) |
| [GetWorkbookJsonWithCache](../../aspose.cells.gridjs/gridjsworkbook/getworkbookjsonwithcache/)(string, string) | Hämtar JSON för hela arbetsboken (med cache) |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_3)(string) | Importerar Excel‑filen från filsökvägen. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile)(Workbook) | Importerar Excel‑filen från Workbook‑objektet. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_1)(Stream, GridLoadFormat) | Importerar Excel‑filen från filström med laddningsformat. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_7)(string, string) | Importerar Excel‑filen från filsökvägen. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_4)(string, Workbook) | Importerar Excel‑filen från Workbook‑objektet. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_2)(Stream, GridLoadFormat, string) | Importerar Excel‑filen från filström med laddningsformat och öppningslösenord. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_5)(string, Stream, GridLoadFormat) | Importerar Excel‑filen från filström. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_8)(string, string, string) | Importerar Excel‑filen från filsökväg och öppningslösenord. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_6)(string, Stream, GridLoadFormat, string) | Importerar Excel‑filen från filström med laddningsformat och öppningslösenord. |
| [ImportExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/importexcelfilefromjson/)(string) | Importerar Excel‑filen från JSON‑formatsträng. |
| [InsertImage](../../aspose.cells.gridjs/gridjsworkbook/insertimage/)(string, string, Stream, string) | Infogar bild i kalkylbladet från filström eller URL (antingen filström eller URL måste tillhandahållas) eller infogar form när p.type är en av AutoShapeType. |
| [JsonToStream](../../aspose.cells.gridjs/gridjsworkbook/jsontostream/)(Stream, string, string) | Generera JSON från den minnesbaserade Workbook och skriv den till den angivna strömmen. Valfritt cachas den genererade JSON för snabbare efterföljande hämtning. Viktiga skillnader mot JsonToStreamByUid: - Denna metod använder det aktuella minnesbaserade Workbook‑tillståndet (wb‑fältet) - JsonToStreamByUid laddar om Workbook från .cells‑cache‑filer på disk - Använd denna metod när du vill exportera det aktuella arbetsbokens tillstånd efter ändringar - Använd JsonToStreamByUid när du behöver återskapa JSON från ett tidigare cachat filtillstånd. Caching‑beteende (när uid tillhandahålls): - Kontrollerar JSON‑cache innan generering (L1‑minne + L2‑disk) - Vid cache‑miss genereras JSON från minnes‑Workbook - Sparar genererad JSON i cache för framtida förfrågningar |
| [JsonToStreamByUid](../../aspose.cells.gridjs/gridjsworkbook/jsontostreambyuid/)(Stream, string, string) | Hämta JSON‑strängen för filen från cachen med angivet unikt id, ange utdatafilnamnet i JSON och skriv den till strömmen. |
| [LazyLoadingJson](../../aspose.cells.gridjs/gridjsworkbook/lazyloadingjson/)(string, string) | Hämtar JSON‑strängen för det angivna bladet i filen från cachen med det angivna unika ID:t. |
| [LazyLoadingStream](../../aspose.cells.gridjs/gridjsworkbook/lazyloadingstream/)(Stream, string, string) | Hämta JSON‑strängen för det angivna bladet i filen från cachen med angivet unikt id och skriv den till strömmen. |
| [MergeExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/mergeexcelfilefromjson/)(string, string) | Tillämpar en batchuppdatering på minnesdata. |
| [RedactFile](../../aspose.cells.gridjs/gridjsworkbook/redactfile/)(string, string, string[]) | Utför redigering på en Excel-fil baserat på en array av JSON-operationer. |
| [SaveToCacheWithFileName](../../aspose.cells.gridjs/gridjsworkbook/savetocachewithfilename/)(string, string, string) | Sparar minnesdata till cache-filen med det angivna filnamnet och sätter även öppningslösenordet, sparformatet baseras på filändelsen för filnamnet. |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile/#savetoexcelfile)(Stream) | Sparar minnesdata till strömmen, baserat på ursprungsfilformatet. |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile/#savetoexcelfile_1)(string) | Sparar minnesdata till filsökvägen, om filen har en filändelse sparas formatet baserat på filändelsen. |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml/#savetohtml)(Stream) | Sparar minnesdata till strömmen, sparformatet är html |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml/#savetohtml_1)(string) | Sparar minnesdata till filsökvägen, sparformatet är html. |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf/#savetopdf)(Stream) | Sparar minnesdata till strömmen, sparformatet är pdf. |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf/#savetopdf_1)(string) | Sparar minnesdata till filsökvägen, sparformatet är pdf. |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx/#savetoxlsx)(Stream) | Sparar minnesdata till strömmen, sparformatet är xlsx. |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx/#savetoxlsx_1)(string) | Sparar minnesdata till filsökvägen, sparformatet är xlsx. |
| [SetInterruptMonitorForLoad](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforload/)(GridInterruptMonitor, int) | Ställer in InterruptMonitor för inläsningsoperation. |
| [SetInterruptMonitorForSave](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforsave/)(GridInterruptMonitor) | Ställer in InterruptMonitor för sparningsoperation. |
| [SetTransParentView](../../aspose.cells.gridjs/gridjsworkbook/settransparentview/)(string, string, bool) | Ställer in transparensen för redigeringsformer i arbetsboken. |
| [TranslateSheetAsync](../../aspose.cells.gridjs/gridjsworkbook/translatesheetasync/)(string, string, ITextTranslator, string) | Översätt alla strängvärden till målspråket i kalkylbladet. |
| [UpdateCell](../../aspose.cells.gridjs/gridjsworkbook/updatecell/)(string, string) | Tillämpar uppdateringsoperationen. |
| static [GetGridLoadFormat](../../aspose.cells.gridjs/gridjsworkbook/getgridloadformat/)(string) | Hämtar inläsningsformatet efter filändelse |
| static [GetImageStream](../../aspose.cells.gridjs/gridjsworkbook/getimagestream/)(string, string, string) | Hämta bildström. |
| static [GetImageUrl](../../aspose.cells.gridjs/gridjsworkbook/getimageurl/)(string, string, string) | Hämtar bildens URL. |
| static [GetUidForFile](../../aspose.cells.gridjs/gridjsworkbook/getuidforfile/)(string) | Genererar ett nytt unikt ID för filcachen med det angivna filnamnet. |
| static [SetImageUrlBase](../../aspose.cells.gridjs/gridjsworkbook/setimageurlbase/)(string) | Ställ in bas-bild-hämtnings-URL:en från kontrollern. |

## Fält

| Namn | Beskrivning |
| --- | --- |
| static [CacheImp](../../aspose.cells.gridjs/gridjsworkbook/cacheimp/) | Anpassad implementation för cachelagring. Om du vill lagra cache i strömformat måste du ställa in och implementera den. |
| static [CalculateEngine](../../aspose.cells.gridjs/gridjsworkbook/calculateengine/) | Anpassad implementation för beräkningsmotor. Om du vill göra anpassade beräkningar måste du ställa in och implementera den. |
| const [pictureType](../../aspose.cells.gridjs/gridjsworkbook/picturetype/) | konstantvärde för bildtypen |
| static [UpdateMonitor](../../aspose.cells.gridjs/gridjsworkbook/updatemonitor/) | Hämtar/Ställer in uppdateringsmonitor för att spåra uppdateringsoperation |

### Se även

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


