---
title: "Delegate CellEventStringHandler"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Hücre olaylarını işlemek amacıyla tasarlanmış yöntemi temsil eder. CellEventHandler arayüzüyle aynı ancak string sonuç döndürür"
type: docs
url: /tr/net/aspose.cells.gridweb.data/celleventstringhandler/
---
## CellEventStringHandler delegate

Hücre olaylarını ele almayı amaçlayan yöntemi temsil eder. CellEventHandler arabirimiyle aynı, ancak string sonuç döndürür.

String **handleCellEvent**(Object sender, CellEventArgs e);

```csharp
public delegate string CellEventStringHandler(object sender, CellEventArgs e);
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sender | Object | Olayın kaynak ızgarası. |
| e | CellEventArgs | Olay argümanı. e.Cell, olayı tetikleyen hücredir. e.Argument, olayın argümanını içerir. |

### Dönüş Değeri

string değer

### Ayrıca Bakınız

* class [CellEventArgs](../../aspose.cells.gridweb/celleventargs/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


