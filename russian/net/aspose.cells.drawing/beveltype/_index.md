---
title: "Перечисление BevelType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.BevelType. Представляет предустановку типа фаски, которую можно применить к фигуре в 3D"
type: docs
url: /ru/net/aspose.cells.drawing/beveltype/
---
## BevelType enumeration

Представляет предустановку типа фаски, которую можно применить к фигуре в 3D.

```csharp
public enum BevelType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Без фаски |
| Angle | `1` | Угол |
| ArtDeco | `2` | Арт-деко |
| Circle | `3` | Круг |
| Convex | `4` | Выпуклый |
| CoolSlant | `5` | Крутой наклон |
| Cross | `6` | Крест |
| Divot | `7` | Вмятина |
| HardEdge | `8` | Жёсткий край |
| RelaxedInset | `9` | Смягчённый отступ |
| Riblet | `10` | Ребристый |
| Slope | `11` | Наклон |
| SoftRound | `12` | Мягко округленный |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class BevelTypeDemo
    {
        public static void BevelTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму на лист
            var shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 100, 100);

            // Получить доступ к 3D-формату формы
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Установите тип и размеры верхней фаски
            threeDFormat.TopBevelType = BevelType.SoftRound;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;

            // Установите тип и размеры нижней фаски
            threeDFormat.BottomBevelType = BevelType.Divot;
            threeDFormat.BottomBevelWidth = 5;
            threeDFormat.BottomBevelHeight = 5;

            // Сохраните книгу
            workbook.Save("BevelTypeExample.xlsx");
            workbook.Save("BevelTypeExample.pdf");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


