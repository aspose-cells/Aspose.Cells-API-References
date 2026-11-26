---
title: "GridCell.SetFont"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GridCell. Устанавливает шрифт в ячейку. Для повышения производительности реализуйте метод SetFont, а не свойство Font."
type: docs
url: /ru/net/aspose.cells.griddesktop.data/gridcell/setfont/
---
## GridCell.SetFont method

Устанавливает шрифт в ячейку. Чтобы улучшить производительность, реализуйте метод "SetFont", а не свойство "Font".

```csharp
public void SetFont(Font font)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| шрифт | Шрифт | шрифт для установки. |

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


