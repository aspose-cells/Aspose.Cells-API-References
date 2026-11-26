---
title: "Делегат CellErrorHandler"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Представляет интерфейс, предназначенный для обработки событий ошибок ячеек"
type: docs
url: /ru/net/aspose.cells.gridweb.data/cellerrorhandler/
---
## CellErrorHandler delegate

Представляет интерфейс, предназначенный для обработки событий ошибок ячеек.

void **handleCellEvent**(Object sender, GridCellException ex, OnErrorActionQuery query);

```csharp
public delegate void CellErrorHandler(object sender, WebCellException ex, 
    OnErrorActionQuery action);
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sender | Object | Источник события. |
| ex | WebCellException | Ошибка операции над ячейкой. |
| действие | OnErrorActionQuery | можно получить информацию о типе действия onerror. |

### См. также

* class [WebCellException](../webcellexception/)
* class [OnErrorActionQuery](../onerroractionquery/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


