---
title: "GridJsWorkbook.InsertImage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "GridJsWorkbook method. Inserisce l'immagine nel foglio di lavoro da un flusso di file o dall'URL; se il flusso di file o l'URL devono essere forniti, oppure inserisce una forma quando p.type è uno dei AutoShapeType"
type: docs
url: /it/net/aspose.cells.gridjs/gridjsworkbook/insertimage/
---
## GridJsWorkbook.InsertImage method

Inserisce un'immagine nel foglio di lavoro da un flusso di file o dall'URL (deve essere fornito o il flusso di file o l'URL), oppure inserisce una forma quando p.type è uno di AutoShapeType.

```csharp
public string InsertImage(string uid, string p, Stream s, string imageUrl)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | String | L'ID univoco per la cache dei file |
| p | String | La stringa JSON in formato per l'operazione che specifica la posizione della cella, il nome del foglio di lavoro, la riga in alto a sinistra, la colonna in alto a sinistra per l'immagine, ecc {name:'sheet1',ri:1,ci:1} |
| s | Stream | Il flusso del file immagine |
| imageUrl | String | L'URL del file immagine |

### Valore di ritorno

La stringa JSON in formato dell'immagine inserita

### Vedi anche

* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


