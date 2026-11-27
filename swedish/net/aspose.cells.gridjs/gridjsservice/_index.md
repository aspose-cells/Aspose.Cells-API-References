---
title: "Klass GridJsService"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridJs.GridJsService-klass. Tillhandahåller de grundläggande operations‑API:erna som används i kontrolleråtgärder"
type: docs
url: /sv/net/aspose.cells.gridjs/gridjsservice/
---
## GridJsService class

Tillhandahåller de grundläggande operations‑API:erna som används i kontrolleråtgärder.

```csharp
public class GridJsService : IGridJsService
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [GridJsService](gridjsservice/#constructor)(GridJsOptions) | Konstruktorn för GridJsService för värdar som själva bygger options‑objektet (webbläsar‑WASM‑värden och alla icke‑DI‑serverinställningar). |
| [GridJsService](gridjsservice/#constructor_1)(IOptions&lt;GridJsOptions&gt;) | Standardkonstruktorn för GridJsService |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Settings](../../aspose.cells.gridjs/gridjsservice/settings/) { get; set; } | Representerar arbetsbokens inställningar. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [AddImage](../../aspose.cells.gridjs/gridjsservice/addimage/#addimage)(string, string, string, byte[]) | Tillämpar operationen för att lägga till bild från lokal fil (filbytes kommer från JS FormData eller någon värd). |
| [AddImage](../../aspose.cells.gridjs/gridjsservice/addimage/#addimage_1)(string, string, string, IFormFileCollection) | Tillämpar operationen för att lägga till bild från lokal fil. |
| [AddImageByURL](../../aspose.cells.gridjs/gridjsservice/addimagebyurl/)(string, string, string) | Tillämpar operationen för att lägga till bild från fjärr-URL. |
| [CheckInCacheForCollaborative](../../aspose.cells.gridjs/gridjsservice/checkincacheforcollaborative/)(string) | Kontrollera om arbetsboksinstansen finns i minnescachen. Denna metod gäller endast för samarbetsläge. |
| [ClearAllJsonCache](../../aspose.cells.gridjs/gridjsservice/clearalljsoncache/)() | Rensar alla JSON-cacheposter (minne och disk). |
| [ClearJsonCacheForUid](../../aspose.cells.gridjs/gridjsservice/clearjsoncacheforuid/)(string) | Rensar alla JSON-cacheposter som tillhör det angivna unika ID:t. Anropa detta efter att ha ändrat källfilen utanför band så att nästa begäran genererar JSON igen. |
| [CopyImage](../../aspose.cells.gridjs/gridjsservice/copyimage/)(string, string) | Tillämpar kopieringsoperationen för bild. |
| [Destroy](../../aspose.cells.gridjs/gridjsservice/destroy/)() | Denna metod är endast för Java, den implementerar destroy‑metoden i DisposableBean, som kommer att anropas automatiskt av Spring när begäran avslutas; faktiskt kommer den att anropa Dispose‑metoden. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid_1)(string, string) | Hämtar JSON‑sträng för filen med det angivna unika ID:t. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid)(Workbook, string, string) | Hämtar JSON‑sträng för arbetsboken med det angivna unika ID:t. |
| [DetailStreamJson](../../aspose.cells.gridjs/gridjsservice/detailstreamjson/#detailstreamjson_1)(Stream, string) | Skriv JSON‑strängen för filen till strömmen. |
| [DetailStreamJson](../../aspose.cells.gridjs/gridjsservice/detailstreamjson/#detailstreamjson)(Stream, Workbook, string) | Skriv JSON‑strängen för arbetsboken till strömmen. |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid_1)(Stream, string, string) | Skriv JSON‑strängen för filen till strömmen med det angivna unika ID:t. |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid)(Stream, Workbook, string, string) | Skriv JSON‑strängen för arbetsboken till strömmen med det angivna unika ID:t. |
| [Dispose](../../aspose.cells.gridjs/gridjsservice/dispose/)() | Utför applikationsdefinierade uppgifter som är kopplade till att frigöra, släppa eller återställa ohanterade resurser. |
| [Download](../../aspose.cells.gridjs/gridjsservice/download/)(string, string, string) | Tillämpar nedladdningsoperationen för fil. |
| [GetFile](../../aspose.cells.gridjs/gridjsservice/getfile/)(string) | Hämta filström. |
| [GetWarningCallback](../../aspose.cells.gridjs/gridjsservice/getwarningcallback/)() | Hämtar anpassad varningsåteruppringning för import av fil. |
| [Image](../../aspose.cells.gridjs/gridjsservice/image/)(string, string) | Hämta bildström. |
| [ImageUrl](../../aspose.cells.gridjs/gridjsservice/imageurl/)(string, string, string) | Hämtar bildens URL. |
| [LazyLoadingJson](../../aspose.cells.gridjs/gridjsservice/lazyloadingjson/)(string, string) | Hämtar JSON‑strängen för det angivna bladet i filen från cachen med det angivna unika ID:t. |
| [LazyLoadingStreamJson](../../aspose.cells.gridjs/gridjsservice/lazyloadingstreamjson/)(Stream, string, string) | Skriver JSON‑strängen för det angivna bladet i filen från cachen med det angivna unika ID:t till strömmen. |
| [Load](../../aspose.cells.gridjs/gridjsservice/load/)(string, string) | Hämtar JSON‑strängen för filen från cachen med det angivna unika ID:t, och sätter utdatafilnamnet i JSON‑en. |
| [Ole](../../aspose.cells.gridjs/gridjsservice/ole/)(string, string, int, out string) | Hämtar byte‑array‑data för det inbäddade OLE‑objektet. |
| [SetWarningCallback](../../aspose.cells.gridjs/gridjsservice/setwarningcallback/)(IWarningCallback) | Ställer in anpassad varningsåteruppringning för import av fil. |
| [TranslateSheetAsync](../../aspose.cells.gridjs/gridjsservice/translatesheetasync/)(string, string, ITextTranslator, string) | Översätt alla strängvärden till målspråket i kalkylbladet. |
| [UpdateCell](../../aspose.cells.gridjs/gridjsservice/updatecell/)(string, string) | Tillämpar uppdateringsoperationen. |

### Se även

* interface [IGridJsService](../igridjsservice/)
* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


