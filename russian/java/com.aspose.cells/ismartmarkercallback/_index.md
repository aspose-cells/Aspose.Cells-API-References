---
title: "ISmartMarkerCallBack"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет интерфейс обратного вызова обработки smartmarker."
type: docs
url: /ru/java/com.aspose.cells/ismartmarkercallback/
---
```
public interface ISmartMarkerCallBack
```

Представляет интерфейс обратного вызова обработки smartmarker.
## Методы

| Метод | Описание |
| --- | --- |
| [process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName)](#process-int-int-int-java.lang.String-java.lang.String-) | Обратный вызов для обработки смарт‑маркировки. |
### process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName) {#process-int-int-int-java.lang.String-java.lang.String-}
```
public abstract void process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName)
```


Обратный вызов для обработки смарт‑маркировки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetIndex | int | Индекс листа. |
| rowIndex | int | Индекс строки. |
| colIndex | int | Индекс столбца. |
| tableName | java.lang.String | Имя таблицы смарт‑маркировки. |
| columnName | java.lang.String | Имя таблицы смарт‑маркировки. |

