---
title: CellEventStringHandler
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет метод предназначенный для обработки событий ячеек. то же что и интерфейс CellEventHandler но возвращает строковый результат
type: docs
weight: 340
url: /ru/net/aspose.cells.griddesktop.data/celleventstringhandler/
---
## CellEventStringHandler delegate

Представляет метод, предназначенный для обработки событий ячеек. то же, что и интерфейс CellEventHandler, но возвращает строковый результат

String **handleCellEvent** ( Отправитель объекта, CellEventArgs e);

```csharp
public delegate string CellEventStringHandler(object sender, CellEventArgs e);
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sender | Object | Исходная сетка события. |
| e | CellEventArgs | Аргумент события. e.Cell — это ячейка, которая инициирует событие. e.Argument содержит аргумент события. |

### Возвращаемое значение

строковое значение

### Смотрите также

* class [CellEventArgs](../../aspose.cells.griddesktop/celleventargs)
* пространство имен [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data)
* сборка [Aspose.Cells.GridDesktop](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->