---
title: "IGridJsJsonCache.GetCacheKey"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo IGridJsJsonCache. Genera una chiave di cache. I clienti possono decidere se includere l'uid in base ai requisiti aziendali. Se conta solo il nome del file, ignora l'uid e usa solo fileName (consigliato) per consentire la condivisione della cache tra lo stesso file. Se è necessario distinguere file con lo stesso nome, usa l'uid in modalità rigorosa"
type: docs
url: /it/net/aspose.cells.gridjs/igridjsjsoncache/getcachekey/
---
## IGridJsJsonCache.GetCacheKey method

Genera una chiave di cache. I clienti possono decidere se includere l'uid in base ai requisiti aziendali. - Se conta solo il nome del file: ignora l'uid e usa solo fileName (consigliato, consente la condivisione della cache tra lo stesso file). - Se è necessario distinguere file con lo stesso nome: usa l'uid (modalità rigorosa).

```csharp
public string GetCacheKey(string uid, string fileName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | String | Identificatore unico del file (può variare per caricamento) |
| fileName | String | Nome file originale |

### Valore di ritorno

Chiave della cache

### Vedi anche

* interface [IGridJsJsonCache](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


