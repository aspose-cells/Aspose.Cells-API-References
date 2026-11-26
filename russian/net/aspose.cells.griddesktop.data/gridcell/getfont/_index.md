---
title: "GridCell.GetFont"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GridCell. Возвращает шрифт ячейки. При изменении шрифта следует вызвать метод SetFont, чтобы установить шрифт для ячейки."
type: docs
url: /ru/net/aspose.cells.griddesktop.data/gridcell/getfont/
---
## GridCell.GetFont method

Получает шрифт ячейки. При изменении шрифта следует вызвать метод "SetFont", чтобы установить шрифт в ячейку.

```csharp
public Font GetFont()
```

### Возвращаемое значение

Возвращает копию шрифта ячейки.

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


