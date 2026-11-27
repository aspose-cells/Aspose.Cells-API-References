---
title: "Gränssnitt IGridJsService"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridJs.IGridJsService-gränssnitt. Representerar det grundläggande operations-API-gränssnittet som används i kontrolleråtgärder"
type: docs
url: /sv/net/aspose.cells.gridjs/igridjsservice/
---
## IGridJsService interface

Representerar det grundläggande operations‑API‑gränssnittet som används i kontrolleråtgärder.

```csharp
public interface IGridJsService : IDisposable
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [AddImage](../../aspose.cells.gridjs/igridjsservice/addimage/#addimage)(string, string, string, byte[]) | Tillämpar operationen för att lägga till bild från lokal fil, genom att ta bildbytarna direkt. |
| [AddImage](../../aspose.cells.gridjs/igridjsservice/addimage/#addimage_1)(string, string, string, IFormFileCollection) | Tillämpar operationen för att lägga till bild från lokal fil, med de uppladdade formulärfilerna. |
| [AddImageByURL](../../aspose.cells.gridjs/igridjsservice/addimagebyurl/)(string, string, string) | Tillämpar operationen för att lägga till bild från fjärr-URL. |
| [CheckInCacheForCollaborative](../../aspose.cells.gridjs/igridjsservice/checkincacheforcollaborative/)(string) | Kontrollera om arbetsboksinstansen finns i minnescachen. Denna metod gäller endast för samarbetsläge. |
| [ClearAllJsonCache](../../aspose.cells.gridjs/igridjsservice/clearalljsoncache/)() | Rensar alla JSON-cacheposter (minne och disk). |
| [ClearJsonCacheForUid](../../aspose.cells.gridjs/igridjsservice/clearjsoncacheforuid/)(string) | Rensar alla JSON-cacheposter som tillhör det angivna unika ID:t. Anropa detta efter att ha ändrat källfilen utanför band så att nästa begäran genererar JSON igen. |
| [CopyImage](../../aspose.cells.gridjs/igridjsservice/copyimage/)(string, string) | Tillämpar kopieringsoperationen för bild. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid_1)(string, string) | Hämtar JSON‑sträng för filen med det angivna unika ID:t. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid)(Workbook, string, string) | Hämtar JSON‑sträng för arbetsboken med det angivna unika ID:t. |
| [DetailStreamJson](../../aspose.cells.gridjs/igridjsservice/detailstreamjson/#detailstreamjson_1)(Stream, string) | Skriv JSON‑strängen för arbetsboken till strömmen. |
| [DetailStreamJson](../../aspose.cells.gridjs/igridjsservice/detailstreamjson/#detailstreamjson)(Stream, Workbook, string) | Skriv JSON‑strängen för arbetsboken till strömmen. |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid_1)(Stream, string, string) | Skriv JSON‑strängen för filen till strömmen med det angivna unika ID:t. |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid)(Stream, Workbook, string, string) | Skriv JSON‑strängen för arbetsboken till strömmen med det angivna unika ID:t. |
| [Download](../../aspose.cells.gridjs/igridjsservice/download/)(string, string, string) | Tillämpar nedladdningsoperationen för fil. |
| [GetFile](../../aspose.cells.gridjs/igridjsservice/getfile/)(string) | Hämta filström. |
| [GetWarningCallback](../../aspose.cells.gridjs/igridjsservice/getwarningcallback/)() | Hämtar anpassad varningsåteruppringning för import av fil. |
| [Image](../../aspose.cells.gridjs/igridjsservice/image/)(string, string) | Hämta bildström. |
| [ImageUrl](../../aspose.cells.gridjs/igridjsservice/imageurl/)(string, string, string) | Hämtar bildens URL. |
| [LazyLoadingJson](../../aspose.cells.gridjs/igridjsservice/lazyloadingjson/)(string, string) | Hämtar JSON‑strängen för det angivna bladet i filen från cachen med det angivna unika ID:t. |
| [LazyLoadingStreamJson](../../aspose.cells.gridjs/igridjsservice/lazyloadingstreamjson/)(Stream, string, string) | Skriver JSON‑strängen för det angivna bladet i filen från cachen med det angivna unika ID:t till strömmen. |
| [Load](../../aspose.cells.gridjs/igridjsservice/load/)(string, string) | Hämtar JSON‑strängen för filen från cachen med det angivna unika ID:t, och sätter utdatafilnamnet i JSON‑en. |
| [Ole](../../aspose.cells.gridjs/igridjsservice/ole/)(string, string, int, out string) | Hämtar byte‑array‑data för det inbäddade OLE‑objektet. |
| [SetWarningCallback](../../aspose.cells.gridjs/igridjsservice/setwarningcallback/)(IWarningCallback) | Ställer in anpassad varningsåteruppringning för import av fil. |
| [UpdateCell](../../aspose.cells.gridjs/igridjsservice/updatecell/)(string, string) | Tillämpar uppdateringsoperationen. |

### Se även

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


