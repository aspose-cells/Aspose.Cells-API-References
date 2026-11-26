---
title: "Перечисление GridRenameStrategy"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.GridDesktop.Data.GridRenameStrategy. Параметр стратегии для дублирующихся имен столбцов"
type: docs
url: /ru/net/aspose.cells.griddesktop.data/gridrenamestrategy/
---
## GridRenameStrategy enumeration

Опция стратегии для дублирования имён столбцов.

```csharp
public enum GridRenameStrategy
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Exception | `0` | Выбрасывает исключение. |
| Digit | `1` | Названо цифрой. Дублированные имена будут выглядеть ...1, ...2 и т.д. |
| Letter | `2` | Названо буквой.. Дублированные имена будут выглядеть ...A, ...B и т.д. |

### Примечания

При обработке данных с заголовками в некоторых сценариях требуется, чтобы заголовки не дублировались во всех столбцах. Например, при экспорте данных в DataTable и необходимости использовать заголовок в качестве имени столбца DataTable, дублирующиеся значения заголовка недопустимы. В подобных ситуациях пользователь может определить, как их обрабатывать, указав эту стратегию.

### См. также

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


