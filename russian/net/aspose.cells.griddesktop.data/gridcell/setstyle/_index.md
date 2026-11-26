---
title: "GridCell.SetStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GridCell. Устанавливает стиль ячейки. Чтобы улучшить производительность, реализуйте метод SetStyle, а не свойство Style"
type: docs
url: /ru/net/aspose.cells.griddesktop.data/gridcell/setstyle/
---
## GridCell.SetStyle method

Устанавливает стиль в ячейку. Чтобы улучшить производительность, реализуйте метод "SetStyle", а не свойство "Style".

```csharp
public void SetStyle(Style value)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| стиль | Стиль | стиль для установки. |

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


