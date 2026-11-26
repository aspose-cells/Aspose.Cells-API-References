---
title: "GridValidation.GetListValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GridValidation. Получает значение списка проверки для указанной ячейки."
type: docs
url: /ru/net/aspose.cells.gridweb.data/gridvalidation/getlistvalue/
---
## GridValidation.GetListValue method

Получить значение списка проверок для указанной ячейки.

```csharp
public object GetListValue(int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки. |
| column | Int32 | Индекс столбца. |

### Возвращаемое значение

Значение для формирования списка этой проверки для указанной ячейки. Если список ссылается на диапазон, возвращаемое значение будет объектом ReferredArea; в противном случае возвращаемое значение может быть null, object[] или простым объектом.

### Примечания

Только для проверки, тип которой List и которая применена к указанной ячейке; в остальных случаях будет возвращено null.

### См. также

* class [GridValidation](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


