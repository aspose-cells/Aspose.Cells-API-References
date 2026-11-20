---
title: "GridCustomServerValidation"
second_title: "Справочник API Aspose.Cells for Java"
description: "Интерфейс, который необходимо реализовать при использовании серверной валидации."
type: docs
url: /ru/java/com.aspose.gridweb/gridcustomservervalidation/
---
```
public interface GridCustomServerValidation
```

интерфейс, который необходимо реализовать при использовании серверной проверки. CustomServerFunction.
## Методы

| Метод | Описание |
| --- | --- |
| [validate(GridWorksheet sheet, int row, int col, String value)](#validate-com.aspose.gridweb.GridWorksheet-int-int-java.lang.String-) | **Примечания** |
### validate(GridWorksheet sheet, int row, int col, String value) {#validate-com.aspose.gridweb.GridWorksheet-int-int-java.lang.String-}
```
public abstract String validate(GridWorksheet sheet, int row, int col, String value)
```


**Remarks**

если вернуть string.empty, проверка считается пройденной, иначе можно вернуть любое связанное сообщение, которое может быть обработано в функции ClientCallback

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | GridWorksheet |
| строка | int | индекс строки ячейки |
| col | int | индекс столбца ячейки |
| значение | java.lang.String | значение для проверки |

**Returns:**
java.lang.String — строковое значение результата
