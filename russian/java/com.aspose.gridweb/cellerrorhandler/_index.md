---
title: "CellErrorHandler"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет интерфейс, предназначенный для обработки событий ошибок ячеек."
type: docs
url: /ru/java/com.aspose.gridweb/cellerrorhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CellErrorHandler extends Serializable
```

Представляет интерфейс, предназначенный для обработки событий ошибок ячеек.
## Методы

| Метод | Описание |
| --- | --- |
| [handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.GridCellException-com.aspose.gridweb.OnErrorActionQuery-) | Обрабатывает связанное событие ячейки. |
### handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.GridCellException-com.aspose.gridweb.OnErrorActionQuery-}
```
public abstract void handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query)
```


Обрабатывает связанное событие ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| отправитель | java.lang.Object | Источник события. |
| ex | [GridCellException](../../com.aspose.gridweb/gridcellexception) | Ошибка операции ячейки. |
| query | [OnErrorActionQuery](../../com.aspose.gridweb/onerroractionquery) | может получить информацию о типе действия onerror. |

