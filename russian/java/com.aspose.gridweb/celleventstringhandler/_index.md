---
title: "CellEventStringHandler"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет интерфейс, предназначенный для обработки событий ячеек."
type: docs
url: /ru/java/com.aspose.gridweb/celleventstringhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CellEventStringHandler extends Serializable
```

Представляет интерфейс, предназначенный для обработки событий ячеек.
## Методы

| Метод | Описание |
| --- | --- |
| [handleCellEvent(Object sender, CellEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-) | Обрабатывает связанное событие ячейки. |
### handleCellEvent(Object sender, CellEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-}
```
public abstract String handleCellEvent(Object sender, CellEventArgs e)
```


Обрабатывает связанное событие ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| отправитель | java.lang.Object | Исходная сетка события. |
| e | [CellEventArgs](../../com.aspose.gridweb/celleventargs) | Аргумент события. e.Cell — ячейка, вызывающая событие. e.Argument содержит аргумент события. |

**Returns:**
java.lang.String — строковое значение
