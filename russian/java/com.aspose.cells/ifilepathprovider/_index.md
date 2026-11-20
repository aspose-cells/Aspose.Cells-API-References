---
title: "IFilePathProvider"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет поставщика пути экспортируемого файла."
type: docs
url: /ru/java/com.aspose.cells/ifilepathprovider/
---
```
public interface IFilePathProvider
```

Представляет поставщика пути экспортируемого файла.
## Методы

| Метод | Описание |
| --- | --- |
| [getFullName(String sheetName)](#getFullName-java.lang.String-) | Получает полный путь к файлу по имени листа при отдельном экспорте листа в HTML. |
### getFullName(String sheetName) {#getFullName-java.lang.String-}
```
public abstract String getFullName(String sheetName)
```


Получает полный путь к файлу по имени листа при отдельном экспорте листа в HTML. Таким образом ссылки между листами могут быть экспортированы корректно.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetName | java.lang.String | Имя листа |

**Returns:**
java.lang.String — полный путь к файлу
