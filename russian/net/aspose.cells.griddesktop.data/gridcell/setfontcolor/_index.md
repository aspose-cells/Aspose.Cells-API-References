---
title: "GridCell.SetFontColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GridCell. Устанавливает цвет шрифта в ячейке. Для повышения производительности реализуйте метод SetFontColor, а не свойство FontColor."
type: docs
url: /ru/net/aspose.cells.griddesktop.data/gridcell/setfontcolor/
---
## GridCell.SetFontColor method

Устанавливает цвет шрифта в ячейке. Чтобы улучшить производительность, реализуйте метод "SetFontColor", а не свойство "FontColor".

```csharp
public void SetFontColor(Color color)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| цвет | Color | цвет шрифта для установки. |

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


