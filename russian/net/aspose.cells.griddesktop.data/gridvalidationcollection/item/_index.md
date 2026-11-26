---
title: "GridValidationCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство GridValidationCollection. Получает элемент Hyperlink по указанному индексу."
type: docs
url: /ru/net/aspose.cells.griddesktop.data/gridvalidationcollection/item/
---
## GridValidationCollection indexer (1 of 2)

Возвращает элемент гиперссылки по указанному индексу.

```csharp
public GridValidation this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс элемента, начиная с нуля. |

### Возвращаемое значение

Элемент по указанному индексу.

### См. также

* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## GridValidationCollection indexer (2 of 2)

Получает элемент [`GridValidation`](../../gridvalidation/) по указанной ячейке. Если проверка отсутствует, возвращает null.

```csharp
public GridValidation this[int row, int column] { get; }
```

| Параметр | Описание |
| --- | --- |
| строка | Строка ячейки. |
| column | Столбец ячейки. |

### Возвращаемое значение

Элемент по указанному индексу.

### Примечания

Если в указанном индексе строки и столбца нет объекта проверки, будет проверяться объект проверки столбца.

### См. также

* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


