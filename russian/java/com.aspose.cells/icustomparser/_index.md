---
title: "ICustomParser"
second_title: "Справочник API Aspose.Cells for Java"
description: "Позволяет пользователям добавить свой пользовательский парсер значений для преобразования строковых значений в другие подходящие объекты значений ячеек."
type: docs
url: /ru/java/com.aspose.cells/icustomparser/
---
```
public interface ICustomParser
```

Позволяет пользователям добавить свой пользовательский парсер значений для преобразования строковых значений в другие подходящие объекты значений ячеек.
## Методы

| Метод | Описание |
| --- | --- |
| [getFormat()](#getFormat--) | Получает шаблон форматирования, соответствующий разобранному значению при последнем вызове [parseObject(String)](../../com.aspose.cells/icustomparser\#parseObject-String-). |
| [parseObject(String value)](#parseObject-java.lang.String-) | Разбирает заданную строку в соответствующий объект значения. |
### getFormat() {#getFormat--}
```
public abstract String getFormat()
```


Получает шаблон форматирования, соответствующий разобранному значению при последнем вызове [parseObject(String)](../../com.aspose.cells/icustomparser\#parseObject-String-).

**Remarks**

Возвращённый шаблон форматирования может быть использован для форматирования соответствующей ячейки (установите Style.Custom для ячейки).

**Returns:**
java.lang.String
### parseObject(String value) {#parseObject-java.lang.String-}
```
public abstract Object parseObject(String value)
```


Разбирает заданную строку в соответствующий объект значения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String | Строковое значение для разбора |

**Returns:**
java.lang.Object — объект значения, полученный из заданной строки. Если строку нельзя разобрать в соответствующий объект значения, возвращается null.
