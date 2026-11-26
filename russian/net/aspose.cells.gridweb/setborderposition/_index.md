---
title: "Перечисление SetBorderPosition"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.GridWeb.SetBorderPosition. Представляет позицию границы, которую нужно установить для диапазона ячеек."
type: docs
url: /ru/net/aspose.cells.gridweb/setborderposition/
---
## SetBorderPosition enumeration

Представляет позицию границы, которую необходимо установить для диапазона ячеек.

```csharp
public enum SetBorderPosition
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Top | `0` | Верхняя граница |
| Bottom | `1` | Нижняя граница |
| Left | `2` | Левая граница |
| Right | `3` | Правая граница |
| HorizontalMiddle | `4` | Нижняя граница |
| VerticalMiddle | `5` | Горизонтальные средние границы |
| Outline | `6` | Границы по вертикальному центру |
| Cross | `7` | Перекрестные границы |
| None | `8` | Без границ |

### Примеры

```csharp
[C#]
    GridWeb GridWeb1=new GridWeb();
	GridWeb1.WorkSheets[0].Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, GridWeb1.WorkSheets[0].Cells[0, 0].Style.LeftBorderStyle);

[VB]
	GridWeb1.WorkSheets(0).Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, GridWeb1.WorkSheets[0].Cells[0, 0].Style.LeftBorderStyle)
```

### См. также

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


