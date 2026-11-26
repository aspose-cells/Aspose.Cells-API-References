---
title: "GridCells.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство GridCells. Получает элемент GridCell по указанному индексу строки и индексу столбца ячейки"
type: docs
url: /ru/net/aspose.cells.gridweb.data/gridcells/item/
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
GridWeb GridWeb1 = new GridWeb();
GridCells cells = GridWeb1.WorkSheets[0].Cells;
//Получает ячейку по адресу "A1".
GridCell cell = cells[0, 0];	

[Visual Basic]

Dim cells As Cells =  excel.WorkSheets(0).Cells
 'Gets the cell at "A1"
Dim cell As Cell =  cells(0,0) 
```

### См. также

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

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

### Примеры

```csharp
[C#]
ridWeb GridWeb1 = new GridWeb();
 GridCells cells = GridWeb1.WorkSheets[0].Cells;
 GridCell cell = cells["A1"];	//Gets the cell at "A1"

[Visual Basic]

Dim cells As Cells =  excel.Worksheets(0).Cells
Dim cell As Cell =  cells("A1")  'Gets the cell at "A1"
```

### См. также

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


