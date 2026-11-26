---
title: "GridCell.GetFontColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "GridCell метод. Получает цвет шрифта ячейки. При изменении цвета следует вызвать метод SetFontColor, чтобы установить цвет шрифта ячейки."
type: docs
url: /ru/net/aspose.cells.griddesktop.data/gridcell/getfontcolor/
---
## GridCell.GetFontColor method

Получает цвет шрифта ячейки. При изменении цвета следует вызвать метод "SetFontColor", чтобы установить цвет шрифта в ячейку.

```csharp
public Color GetFontColor()
```

### Возвращаемое значение

возвращает цвет шрифта ячейки.

### Примеры

```csharp
[C#]
GridCell cell = gridDesktop1.GetActiveWorksheet().Cells[0, 0];
Font font = new Font("Courier New", 8, FontStyle.Italic);
cell.SetFont(font);
Color color = cell.GetFontColor();
color = Color.Black;
cell.SetFontColor(color);

[Visual Basic]
Dim cell As GridCell =  gridDesktop1.GetActiveWorksheet().Cells(0, 0) 
Dim font As Font =  New Font("Courier New",8,FontStyle.Italic) 
cell.SetFont(font)
Dim color As Color =  cell.GetFontColor() 
color = Color.Black
cell.SetFontColor(color)

```

### См. также

* class [GridCell](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


