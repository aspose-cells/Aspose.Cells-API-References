---
title: "Delege CellErrorHandler"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Hücre hata olaylarını ele almayı amaçlayan arayüzü temsil eder"
type: docs
url: /tr/net/aspose.cells.gridweb.data/cellerrorhandler/
---
## CellErrorHandler delegate

Hücre hata olaylarını ele almayı amaçlayan arabirimi temsil eder.

void **handleCellEvent**(Object sender, GridCellException ex, OnErrorActionQuery query);

```csharp
public delegate void CellErrorHandler(object sender, WebCellException ex, 
    OnErrorActionQuery action);
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sender | Object | Olayın kaynağı. |
| ex | WebCellException | Hücre işlem hatası. |
| eylem | OnErrorActionQuery | onerror eylem türü bilgisi alınabilir. |

### Ayrıca Bakınız

* class [WebCellException](../webcellexception/)
* class [OnErrorActionQuery](../onerroractionquery/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


