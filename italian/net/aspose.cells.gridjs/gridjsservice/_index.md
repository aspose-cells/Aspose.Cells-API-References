---
title: "Classe GridJsService"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridJs.GridJsService. Fornisce le API operative di base utilizzate nelle azioni del controller"
type: docs
url: /it/net/aspose.cells.gridjs/gridjsservice/
---
## GridJsService class

Fornisce le API operative di base utilizzate nelle azioni del controller.

```csharp
public class GridJsService : IGridJsService
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [GridJsService](gridjsservice/#constructor)(GridJsOptions) | Il costruttore per GridJsService per gli host che creano l'oggetto delle opzioni autonomamente (l'host browser WASM e qualsiasi configurazione server non DI). |
| [GridJsService](gridjsservice/#constructor_1)(IOptions&lt;GridJsOptions&gt;) | Il costruttore predefinito per GridJsService |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Settings](../../aspose.cells.gridjs/gridjsservice/settings/) { get; set; } | Rappresenta le impostazioni del workbook. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddImage](../../aspose.cells.gridjs/gridjsservice/addimage/#addimage)(string, string, string, byte[]) | Esegue l'operazione di aggiunta immagine da file locale (i byte del file provengono da JS FormData o da qualsiasi host). |
| [AddImage](../../aspose.cells.gridjs/gridjsservice/addimage/#addimage_1)(string, string, string, IFormFileCollection) | Esegue l'operazione di aggiunta immagine da file locale. |
| [AddImageByURL](../../aspose.cells.gridjs/gridjsservice/addimagebyurl/)(string, string, string) | Esegue l'operazione di aggiunta immagine da URL remoto. |
| [CheckInCacheForCollaborative](../../aspose.cells.gridjs/gridjsservice/checkincacheforcollaborative/)(string) | Verifica se l'istanza della cartella di lavoro è nella cache di memoria. Questo metodo è applicabile solo in modalità Collaborativa. |
| [ClearAllJsonCache](../../aspose.cells.gridjs/gridjsservice/clearalljsoncache/)() | Cancella tutte le voci della cache JSON (memoria e disco). |
| [ClearJsonCacheForUid](../../aspose.cells.gridjs/gridjsservice/clearjsoncacheforuid/)(string) | Cancella tutte le voci della cache JSON appartenenti all'ID univoco specificato. Esegui questa operazione dopo aver modificato il file sorgente al di fuori del flusso normale, così la prossima richiesta rigenera il JSON. |
| [CopyImage](../../aspose.cells.gridjs/gridjsservice/copyimage/)(string, string) | Esegue l'operazione di copia immagine. |
| [Destroy](../../aspose.cells.gridjs/gridjsservice/destroy/)() | Questo metodo è solo per Java, implementa il metodo destroy in DisposableBean, che verrà chiamato automaticamente da Spring al termine della richiesta; in realtà chiamerà il metodo Dispose. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid_1)(string, string) | Ottiene la stringa JSON per il file tramite l'ID univoco specificato. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid)(Workbook, string, string) | Ottiene la stringa JSON per la cartella di lavoro tramite l'ID univoco specificato. |
| [DetailStreamJson](../../aspose.cells.gridjs/gridjsservice/detailstreamjson/#detailstreamjson_1)(Stream, string) | Scrive la stringa JSON del file nello stream. |
| [DetailStreamJson](../../aspose.cells.gridjs/gridjsservice/detailstreamjson/#detailstreamjson)(Stream, Workbook, string) | Scrive la stringa JSON della cartella di lavoro nello stream |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid_1)(Stream, string, string) | Scrive la stringa JSON del file nello stream tramite l'ID univoco specificato. |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid)(Stream, Workbook, string, string) | Scrive la stringa JSON della cartella di lavoro nello stream tramite l'ID univoco specificato. |
| [Dispose](../../aspose.cells.gridjs/gridjsservice/dispose/)() | Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al reset delle risorse non gestite. |
| [Download](../../aspose.cells.gridjs/gridjsservice/download/)(string, string, string) | Applica l'operazione di download del file |
| [GetFile](../../aspose.cells.gridjs/gridjsservice/getfile/)(string) | Ottieni lo stream del file |
| [GetWarningCallback](../../aspose.cells.gridjs/gridjsservice/getwarningcallback/)() | Ottiene la callback di avviso personalizzata per l'importazione del file. |
| [Image](../../aspose.cells.gridjs/gridjsservice/image/)(string, string) | Ottieni lo stream dell'immagine. |
| [ImageUrl](../../aspose.cells.gridjs/gridjsservice/imageurl/)(string, string, string) | Ottiene l'URL dell'immagine. |
| [LazyLoadingJson](../../aspose.cells.gridjs/gridjsservice/lazyloadingjson/)(string, string) | Ottiene la stringa JSON del foglio specificato nel file dalla cache usando l'ID univoco specificato. |
| [LazyLoadingStreamJson](../../aspose.cells.gridjs/gridjsservice/lazyloadingstreamjson/)(Stream, string, string) | Scrive la stringa JSON del foglio specificato nel file dalla cache usando l'ID univoco specificato nello stream.. |
| [Load](../../aspose.cells.gridjs/gridjsservice/load/)(string, string) | Ottiene la stringa JSON del file dalla cache usando l'ID univoco specificato, imposta il nome file di output nel JSON. |
| [Ole](../../aspose.cells.gridjs/gridjsservice/ole/)(string, string, int, out string) | Ottiene i dati dell'array di byte dell'oggetto OLE incorporato. |
| [SetWarningCallback](../../aspose.cells.gridjs/gridjsservice/setwarningcallback/)(IWarningCallback) | Imposta la callback di avviso personalizzata per l'importazione del file. |
| [TranslateSheetAsync](../../aspose.cells.gridjs/gridjsservice/translatesheetasync/)(string, string, ITextTranslator, string) | Traduci tutti i valori stringa nella lingua di destinazione nel foglio di lavoro |
| [UpdateCell](../../aspose.cells.gridjs/gridjsservice/updatecell/)(string, string) | Applica l'operazione di aggiornamento. |

### Vedi anche

* interface [IGridJsService](../igridjsservice/)
* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


