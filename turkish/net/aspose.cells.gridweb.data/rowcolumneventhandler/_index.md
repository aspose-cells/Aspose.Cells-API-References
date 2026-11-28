---
title: "Delegate RowColumnEventHandler"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Satır/sütun olaylarını ele almayı amaçlayan arayüzü temsil eder"
type: docs
url: /tr/net/aspose.cells.gridweb.data/rowcolumneventhandler/
---
## RowColumnEventHandler delegate

Satır/sütun olaylarını ele almayı amaçlayan arayüzü temsil eder.

void **handleCellEvent**(Object sender, RowColumnEventArgs e);

```csharp
public delegate void RowColumnEventHandler(object sender, RowColumnEventArgs e);
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sender | Object | Olayın kaynağı. |
| e | RowColumnEventArgs | Olay argümanı. RowDeleting veya ColumnDeleting olay işleyicilerinde silme işlemini iptal etmek istiyorsanız e.RejectOperation() çağırın. |

### Ayrıca Bakınız

* class [RowColumnEventArgs](../../aspose.cells.gridweb/rowcolumneventargs/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


