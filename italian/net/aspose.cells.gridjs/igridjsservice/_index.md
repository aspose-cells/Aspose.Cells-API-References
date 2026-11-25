---
title: "Interfaccia IGridJsService"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Interfaccia Aspose.Cells.GridJs.IGridJsService. Rappresenta l'interfaccia di base delle API operative utilizzata nelle azioni del controller"
type: docs
url: /it/net/aspose.cells.gridjs/igridjsservice/
---
## IGridJsService interface

Rappresenta l'interfaccia delle API operative di base utilizzate nelle azioni del controller.

```csharp
public interface IGridJsService : IDisposable
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddImage](../../aspose.cells.gridjs/igridjsservice/addimage/#addimage)(string, string, string, byte[]) | Applica l'operazione di aggiunta immagine da file locale, prendendo i byte dell'immagine direttamente. |
| [AddImage](../../aspose.cells.gridjs/igridjsservice/addimage/#addimage_1)(string, string, string, IFormFileCollection) | Applica l'operazione di aggiunta immagine da file locale, prendendo i file del modulo caricati. |
| [AddImageByURL](../../aspose.cells.gridjs/igridjsservice/addimagebyurl/)(string, string, string) | Esegue l'operazione di aggiunta immagine da URL remoto. |
| [CheckInCacheForCollaborative](../../aspose.cells.gridjs/igridjsservice/checkincacheforcollaborative/)(string) | Verifica se l'istanza della cartella di lavoro è nella cache di memoria. Questo metodo è applicabile solo in modalità Collaborativa. |
| [ClearAllJsonCache](../../aspose.cells.gridjs/igridjsservice/clearalljsoncache/)() | Cancella tutte le voci della cache JSON (memoria e disco). |
| [ClearJsonCacheForUid](../../aspose.cells.gridjs/igridjsservice/clearjsoncacheforuid/)(string) | Cancella tutte le voci della cache JSON appartenenti all'ID univoco specificato. Esegui questa operazione dopo aver modificato il file sorgente al di fuori del flusso normale, così la prossima richiesta rigenera il JSON. |
| [CopyImage](../../aspose.cells.gridjs/igridjsservice/copyimage/)(string, string) | Esegue l'operazione di copia immagine. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid_1)(string, string) | Ottiene la stringa JSON per il file tramite l'ID univoco specificato. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid)(Workbook, string, string) | Ottiene la stringa JSON per la cartella di lavoro tramite l'ID univoco specificato. |
| [DetailStreamJson](../../aspose.cells.gridjs/igridjsservice/detailstreamjson/#detailstreamjson_1)(Stream, string) | Scrive la stringa JSON della cartella di lavoro nello stream |
| [DetailStreamJson](../../aspose.cells.gridjs/igridjsservice/detailstreamjson/#detailstreamjson)(Stream, Workbook, string) | Scrive la stringa JSON della cartella di lavoro nello stream |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid_1)(Stream, string, string) | Scrive la stringa JSON del file nello stream tramite l'ID univoco specificato. |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid)(Stream, Workbook, string, string) | Scrive la stringa JSON della cartella di lavoro nello stream tramite l'ID univoco specificato. |
| [Download](../../aspose.cells.gridjs/igridjsservice/download/)(string, string, string) | Applica l'operazione di download del file |
| [GetFile](../../aspose.cells.gridjs/igridjsservice/getfile/)(string) | Ottieni lo stream del file |
| [GetWarningCallback](../../aspose.cells.gridjs/igridjsservice/getwarningcallback/)() | Ottiene la callback di avviso personalizzata per l'importazione del file. |
| [Image](../../aspose.cells.gridjs/igridjsservice/image/)(string, string) | Ottieni lo stream dell'immagine. |
| [ImageUrl](../../aspose.cells.gridjs/igridjsservice/imageurl/)(string, string, string) | Ottiene l'URL dell'immagine. |
| [LazyLoadingJson](../../aspose.cells.gridjs/igridjsservice/lazyloadingjson/)(string, string) | Ottiene la stringa JSON del foglio specificato nel file dalla cache usando l'ID univoco specificato. |
| [LazyLoadingStreamJson](../../aspose.cells.gridjs/igridjsservice/lazyloadingstreamjson/)(Stream, string, string) | Scrive la stringa JSON del foglio specificato nel file dalla cache usando l'ID univoco specificato nello stream.. |
| [Load](../../aspose.cells.gridjs/igridjsservice/load/)(string, string) | Ottiene la stringa JSON del file dalla cache usando l'ID univoco specificato, imposta il nome file di output nel JSON. |
| [Ole](../../aspose.cells.gridjs/igridjsservice/ole/)(string, string, int, out string) | Ottiene i dati dell'array di byte dell'oggetto OLE incorporato. |
| [SetWarningCallback](../../aspose.cells.gridjs/igridjsservice/setwarningcallback/)(IWarningCallback) | Imposta la callback di avviso personalizzata per l'importazione del file. |
| [UpdateCell](../../aspose.cells.gridjs/igridjsservice/updatecell/)(string, string) | Applica l'operazione di aggiornamento. |

### Vedi anche

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


