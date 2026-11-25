---
title: "GridJsWorkbook.JsonToStream"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GridJsWorkbook. Genera JSON dal Workbook in memoria e lo scrive nello stream specificato. Opzionalmente memorizza nella cache il JSON generato per un recupero più rapido successivo. Differenze principali rispetto a JsonToStreamByUid: questo metodo utilizza lo stato corrente del Workbook in memoria (campo wb). JsonToStreamByUid ricarica il Workbook dai file di cache .cells su disco. Usa questo metodo quando desideri esportare lo stato attuale del workbook dopo le modifiche. Usa JsonToStreamByUid quando devi rigenerare JSON da uno stato di file precedentemente memorizzato nella cache. Comportamento della cache quando viene fornito un uid: controlla la cache JSON prima di generare (L1 memoria, L2 disco). Se la cache non è presente, genera JSON dal workbook in memoria. Memorizza il JSON generato nella cache per richieste future."
type: docs
url: /it/net/aspose.cells.gridjs/gridjsworkbook/jsontostream/
---
## GridJsWorkbook.JsonToStream method

Genera JSON dal Workbook in memoria e lo scrive nello stream specificato. Opzionalmente memorizza nella cache il JSON generato per un recupero più rapido successivo. Differenze principali rispetto a JsonToStreamByUid: - Questo metodo utilizza lo stato attuale del Workbook in memoria (campo wb) - JsonToStreamByUid ricarica il Workbook dai file di cache .cells su disco - Usa questo metodo quando vuoi esportare lo stato corrente del workbook dopo le modifiche - Usa JsonToStreamByUid quando devi rigenerare JSON da uno stato di file precedentemente memorizzato nella cache. Comportamento della cache (quando uid è fornito): - Controlla la cache JSON prima di generare (memoria L1 + disco L2) - In caso di cache miss, genera JSON dal workbook in memoria - Salva il JSON generato nella cache per richieste future

```csharp
public void JsonToStream(Stream stream, string filename, string uid = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Lo stream di output su cui scrivere i dati JSON. |
| filename | String | Specifica il nome del file nel JSON. Se impostato a null, il nome file predefinito è: book1. |
| uid | String | Identificatore univoco opzionale per la cache JSON. Quando fornito, abilita la ricerca e la memorizzazione nella cache. |

### Vedi anche

* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


