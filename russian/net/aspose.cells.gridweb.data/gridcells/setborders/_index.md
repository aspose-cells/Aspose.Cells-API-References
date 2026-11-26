---
title: "GridCells.SetBorders"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GridCells. Устанавливает границы для диапазона ячеек"
type: docs
url: /ru/net/aspose.cells.gridweb.data/gridcells/setborders/
---
## GridCells.SetBorders method

Устанавливает границы для диапазона ячеек.

```csharp
public void SetBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, 
    SetBorderPosition position, WebBorderStyle borderStyle)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | Int32 | Номер первой строки диапазона (нумерация с нуля). |
| firstColumn | Int32 | Номер первого столбца диапазона (нумерация с нуля). |
| rowNumber | Int32 | Количество строк. |
| columnNumber | Int32 | Количество столбцов. |
| позиция | SetBorderPosition | Позиция границы. |
| borderStyle | WebBorderStyle | Стиль границы. |

### Примеры

```csharp
[C#]
  GridWeb GridWeb1 = new GridWeb();
  WebBorderStyle borderStyle1 = new WebBorderStyle();
 GridWeb1.WorkSheets[0].Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, borderStyle1);

[VB]
	GridWeb1.WebWorksheets(0).Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, borderStyle1)
```

### См. также

* enum [SetBorderPosition](../../../aspose.cells.gridweb/setborderposition/)
* class [WebBorderStyle](../../../aspose.cells.gridweb/webborderstyle/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


