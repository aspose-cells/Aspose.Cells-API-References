---
title: "WebCells.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "WebCells свойство. Получает элемент Cell по указанному индексу строки и индексу столбца ячейки"
type: docs
url: /ru/net/aspose.cells.gridweb.data/webcells/item/
---
## WebCells indexer (1 of 2)

Получает элемент Cell по указанному индексу строки и индексу столбца ячейки.

```csharp
public WebCell this[int row, int column] { get; }
```

| Параметр | Описание |
| --- | --- |
| строка | Индекс строки. |
| column | Индекс столбца. |

### Возвращаемое значение

Объект Cell.

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

* class [WebCell](../../webcell/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## WebCells indexer (2 of 2)

Получает элемент Cell по указанному имени ячейки.

```csharp
public WebCell this[string cellName] { get; }
```

| Параметр | Описание |
| --- | --- |
| cellName | Имя ячейки, включая её букву столбца и номер строки, например A5. |

### Возвращаемое значение

Объект Cell

### Примеры

```csharp
[C#]

Cells cells = excel.Worksheets[0].Cells;
Cell cell = cells["A1"];	//Gets the cell at "A1"

[Visual Basic]

Dim cells As Cells =  excel.Worksheets(0).Cells
Dim cell As Cell =  cells("A1")  'Gets the cell at "A1"
```

### См. также

* class [WebCell](../../webcell/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


