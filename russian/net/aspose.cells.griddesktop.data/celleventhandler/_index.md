---
title: "Делегат CellEventHandler"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Представляет интерфейс, предназначенный для обработки событий ячеек"
type: docs
url: /ru/net/aspose.cells.griddesktop.data/celleventhandler/
---
## CellEventHandler delegate

Представляет интерфейс, предназначенный для обработки событий ячеек.

void **handleCellEvent**(Object sender, CellEventArgs e);

```csharp
public delegate void CellEventHandler(object sender, CellEventArgs e);
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sender | Object | Исходная сетка события. |
| e | CellEventArgs | Аргумент события. e.Cell — это ячейка, вызывающая событие. e.Argument содержит аргумент события. |

### См. также

* class [CellEventArgs](../../aspose.cells.griddesktop/celleventargs/)
* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


