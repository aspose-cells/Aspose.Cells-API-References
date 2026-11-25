---
title: "Interfaccia IGridJsJsonCache"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Interfaccia Aspose.Cells.GridJs.IGridJsJsonCache. Interfaccia di cache JSON che i clienti implementano con strategie specifiche di archiviazione e invalidazione"
type: docs
url: /it/net/aspose.cells.gridjs/igridjsjsoncache/
---
## IGridJsJsonCache interface

Interfaccia della cache JSON - i clienti implementano strategie di archiviazione e invalidazione specifiche

```csharp
public interface IGridJsJsonCache
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| [ClearAll](../../aspose.cells.gridjs/igridjsjsoncache/clearall/)() | Cancella tutte le cache |
| [GetCacheKey](../../aspose.cells.gridjs/igridjsjsoncache/getcachekey/)(string, string) | Genera una chiave di cache. I clienti possono decidere se includere l'uid in base ai requisiti aziendali. - Se conta solo il nome del file: ignora l'uid e usa solo fileName (consigliato, consente la condivisione della cache tra lo stesso file). - Se è necessario distinguere file con lo stesso nome: usa l'uid (modalità rigorosa). |
| [Invalidate](../../aspose.cells.gridjs/igridjsjsoncache/invalidate/)(string) | Invalidare la voce di cache specificata. |
| [InvalidateAllForUid](../../aspose.cells.gridjs/igridjsjsoncache/invalidateallforuid/)(string) | Invalidare tutte le voci di cache contenenti l'uid specificato. Questo è utile quando non si conosce il fileName esatto utilizzato per la cache. |
| [SetJson](../../aspose.cells.gridjs/igridjsjsoncache/setjson/)(string, string) | Scrivi JSON nella cache. |
| [TryGetJson](../../aspose.cells.gridjs/igridjsjsoncache/trygetjson/)(string) | Tentativo di recuperare JSON dalla cache. |

### Vedi anche

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


