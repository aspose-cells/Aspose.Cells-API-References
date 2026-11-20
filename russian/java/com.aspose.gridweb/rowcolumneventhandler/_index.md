---
title: "RowColumnEventHandler"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет интерфейс, предназначенный для обработки событий строк/столбцов."
type: docs
url: /ru/java/com.aspose.gridweb/rowcolumneventhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface RowColumnEventHandler extends Serializable
```

Представляет интерфейс, предназначенный для обработки событий строк/столбцов.
## Методы

| Метод | Описание |
| --- | --- |
| [handleCellEvent(Object sender, RowColumnEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.RowColumnEventArgs-) | Обрабатывает связанное событие ячейки. |
### handleCellEvent(Object sender, RowColumnEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.RowColumnEventArgs-}
```
public abstract void handleCellEvent(Object sender, RowColumnEventArgs e)
```


Обрабатывает связанное событие ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| отправитель | java.lang.Object | Источник события. |
| e | [RowColumnEventArgs](../../com.aspose.gridweb/rowcolumneventargs) | Аргумент события. Вызовите e.RejectOperation(), если хотите отменить операцию удаления в обработчиках событий RowDeleting или ColumnDeleting. |

