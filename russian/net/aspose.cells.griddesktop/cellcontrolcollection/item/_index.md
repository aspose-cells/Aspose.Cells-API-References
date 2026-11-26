---
title: "CellControlCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "CellControlCollection свойство. Получает управление ячейкой по указанному индексу строки и столбца."
type: docs
url: /ru/net/aspose.cells.griddesktop/cellcontrolcollection/item/
---
## CellControlCollection indexer (1 of 2)

Получает управление ячейкой по указанному индексу строки и столбца.

```csharp
public CellControl this[int row, int col] { get; }
```

| Параметр | Описание |
| --- | --- |
| строка | индекс строки. |
| col | индекс столбца. |

### Примечания

Если в указанном индексе строки и столбца нет объекта CellControl, будет проверен объект CellControl столбца.

### См. также

* class [CellControl](../../cellcontrol/)
* class [CellControlCollection](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## CellControlCollection indexer (2 of 2)

Получает управление ячейкой по указанному имени ячейки.

```csharp
public CellControl this[string cellName] { get; }
```

| Параметр | Описание |
| --- | --- |
| cellName | имя ячейки (в формате Excel, например 'A1', 'F22') |

### Примечания

Если в указанном индексе строки и столбца нет объекта CellControl, будет проверен объект CellControl столбца.

### См. также

* class [CellControl](../../cellcontrol/)
* class [CellControlCollection](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


