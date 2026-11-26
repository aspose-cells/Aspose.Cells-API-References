---
title: "Делегат CellEventStringHandler"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Представляет метод, предназначенный для обработки событий ячеек. То же, что интерфейс CellEventHandler, но возвращает строковый результат."
type: docs
url: /ru/net/aspose.cells.griddesktop.data/celleventstringhandler/
---
## CellEventStringHandler delegate

Представляет метод, предназначенный для обработки событий ячеек. Аналогичен интерфейсу CellEventHandler, но возвращает строковый результат.

String **handleCellEvent**(Object sender, CellEventArgs e);

```csharp
public delegate string CellEventStringHandler(object sender, CellEventArgs e);
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sender | Object | Исходная сетка события. |
| e | CellEventArgs | Аргумент события. e.Cell — это ячейка, вызывающая событие. e.Argument содержит аргумент события. |

### Возвращаемое значение

строковое значение

### См. также

* class [CellEventArgs](../../aspose.cells.griddesktop/celleventargs/)
* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


