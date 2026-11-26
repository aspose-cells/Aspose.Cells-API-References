---
title: "GridCells.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство GridCells. Получает элемент GridCell по указанному индексу строки и индексу столбца ячейки"
type: docs
url: /ru/net/aspose.cells.griddesktop.data/gridcells/item/
---
## GridCells indexer (1 of 2)

Получает элемент [`GridCell`](../../gridcell/) по указанному индексу строки и индексу столбца ячейки.

```csharp
public GridCell this[int row, int column] { get; }
```

| Параметр | Описание |
| --- | --- |
| строка | Индекс строки. |
| column | Индекс столбца. |

### Возвращаемое значение

Объект [`GridCell`](../../gridcell/).

### Примеры

```csharp
[C#]

Cells cells = excel.Worksheets[0].Cells;
Cell cell = cells[0, 0];	//Gets the cell at "A1"

[Visual Basic]

Dim cells As Cells =  excel.WorkSheets(0).Cells
Dim cell As Cell =  cells(0,0)  'Gets the cell at "A1"
```

### См. также

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## GridCells indexer (2 of 2)

Получает элемент [`GridCell`](../../gridcell/) по указанному имени ячейки.

```csharp
public GridCell this[string cellName] { get; }
```

| Параметр | Описание |
| --- | --- |
| cellName | Имя ячейки, включая её букву столбца и номер строки, например A5. |

### Возвращаемое значение

Объект [`GridCell`](../../gridcell/)

### См. также

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


