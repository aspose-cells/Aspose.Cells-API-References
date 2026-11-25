---
title: "GridJsService.AddImage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GridJsService. Applica l'aggiunta dell'immagine da file locale; i byte del file provengono da JS FormData o da qualsiasi host"
type: docs
url: /it/net/aspose.cells.gridjs/gridjsservice/addimage/
---
## AddImage(string, string, string, byte[]) {#addimage}

Esegue l'operazione di aggiunta immagine da file locale (i byte del file provengono da JS FormData o da qualsiasi host).

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

* class [GridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## AddImage(string, string, string, IFormFileCollection) {#addimage_1}

Esegue l'operazione di aggiunta immagine da file locale.

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

* class [GridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


