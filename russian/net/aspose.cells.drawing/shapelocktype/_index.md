---
title: "Перечисление ShapeLockType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.ShapeLockType. Представляет тип свойства, которое будет заблокировано"
type: docs
url: /ru/net/aspose.cells.drawing/shapelocktype/
---
## ShapeLockType enumeration

Представляет тип свойства, которое будет заблокировано.

```csharp
public enum ShapeLockType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Group | `0` | Группа |
| AdjustHandles | `1` | AdjustHandles |
| Text | `2` | Текст |
| Points | `3` | Points |
| Crop | `4` | Crop |
| Selection | `5` | Selection |
| Move | `6` | Move |
| AspectRatio | `7` | AspectRatio |
| Rotation | `8` | Rotation |
| Ungroup | `9` | Ungroup |
| Resize | `10` | Resize |
| ShapeType | `11` | ShapeType |
| Arrowhead | `12` | Arrowhead |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShapeLockTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить изображение на лист
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[index];

            // Продемонстрировать функциональность ShapeLockType
            picture.SetLockedProperty(Aspose.Cells.Drawing.ShapeLockType.AspectRatio, false);
            bool isAspectRatioLocked = picture.GetLockedProperty(Aspose.Cells.Drawing.ShapeLockType.AspectRatio);

            Console.WriteLine("Aspect Ratio locked: " + isAspectRatioLocked);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


