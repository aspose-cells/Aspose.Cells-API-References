---
title: "GridCell.GetStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GridCell. Возвращает стиль ячейки. При изменении стиля следует вызвать метод SetStyle, чтобы установить стиль для ячейки."
type: docs
url: /ru/net/aspose.cells.griddesktop.data/gridcell/getstyle/
---
## GridCell.GetStyle method

Получает стиль ячейки. При изменении стиля следует вызвать метод "SetStyle", чтобы установить стиль в ячейку.

```csharp
public Style GetStyle()
```

### Возвращаемое значение

Возвращает копию стиля ячейки.

### Примеры

```csharp
[C#]
Style style = sheet.GetCell(0, 0).GetStyle();
style.CellLocked = true;
style.VAlignment = VerticalAlignmentType.Top;
...
sheet.GetCell(0, 0).SetStyle(style);

[Visual Basic]
Dim style As Style =  sheet.GetCell(0,0).GetStyle() 
style.CellLocked = True
style.VAlignment = VerticalAlignmentType.Top
...
sheet.GetCell(0, 0).SetStyle(style)

```

### См. также

* class [Style](../../../aspose.cells.griddesktop/style/)
* class [GridCell](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


