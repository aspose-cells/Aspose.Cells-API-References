---
title: "IGridJsService.AddImage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo IGridJsService. Applica l'operazione di aggiunta immagine da file locale prendendo direttamente i byte dell'immagine"
type: docs
url: /it/net/aspose.cells.gridjs/igridjsservice/addimage/
---
## AddImage(string, string, string, byte[]) {#addimage}

Applica l'operazione di aggiunta immagine da file locale, prendendo i byte dell'immagine direttamente.

```csharp
public string AddImage(string p, string uid, string iscontrol, byte[] fileBytes)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| p | String | Il parametro stringa JSON |
| uid | String | L'ID univoco per la cache del file. |
| iscontrol | String | Specifica se è un controllo. |
| fileBytes | Byte[] | I byte grezzi del file immagine |

### Valore di ritorno

Il risultato stringa JSON

### Vedi anche

* interface [IGridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## AddImage(string, string, string, IFormFileCollection) {#addimage_1}

Applica l'operazione di aggiunta immagine da file locale, prendendo i file del modulo caricati.

```csharp
public string AddImage(string p, string uid, string iscontrol, IFormFileCollection files)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| p | String | Il parametro stringa JSON |
| uid | String | L'ID univoco per la cache del file. |
| iscontrol | String | Specifica se è un controllo. |
| file | IFormFileCollection | Il file del modulo dell'immagine |

### Valore di ritorno

Il risultato stringa JSON

### Vedi anche

* interface [IGridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


