---
title: "WorkbookEventHandler"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет интерфейс, предназначенный для обработки событий книги."
type: docs
url: /ru/java/com.aspose.gridweb/workbookeventhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface WorkbookEventHandler extends Serializable
```

Представляет интерфейс, предназначенный для обработки событий книги.
## Методы

| Метод | Описание |
| --- | --- |
| [handleCellEvent(Object sender, CellEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-) | Обрабатывает связанное событие ячейки. |
### handleCellEvent(Object sender, CellEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-}
```
public abstract void handleCellEvent(Object sender, CellEventArgs e)
```


Обрабатывает связанное событие ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| отправитель | java.lang.Object | Источник события. |
| e | [CellEventArgs](../../com.aspose.gridweb/celleventargs) | Аргумент события. |

