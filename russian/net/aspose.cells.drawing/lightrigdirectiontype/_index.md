---
title: "Перечисление LightRigDirectionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.LightRigDirectionType enum. Представляет тип направления светового рига"
type: docs
url: /ru/net/aspose.cells.drawing/lightrigdirectiontype/
---
## LightRigDirectionType enumeration

Представляет тип направления световой установки.

```csharp
public enum LightRigDirectionType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Bottom | `0` | Низ |
| BottomLeft | `1` | Снизу слева. |
| BottomRight | `2` | Низ правый. |
| Left | `3` | Слева. |
| Right | `4` | Вправо. |
| Top | `5` | Сверху. |
| TopLeft | `6` | Сверху слева. |
| TopRight | `7` | Сверху справа. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassLightRigDirectionTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте фигуру, чтобы продемонстрировать направление световой установки
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 10, 10, 200, 200, 0, 0);

            // Установите направление световой установки для 3D‑формата фигуры
            shape.ThreeDFormat.LightingDirection = LightRigDirectionType.TopRight;

            // Продемонстрируйте разные направления световой установки
            Console.WriteLine("Current Light Rig Direction: " + shape.ThreeDFormat.LightingDirection);

            // Измените направление световой установки
            shape.ThreeDFormat.LightingDirection = LightRigDirectionType.BottomLeft;
            Console.WriteLine("Changed Light Rig Direction: " + shape.ThreeDFormat.LightingDirection);

            // Переберите все возможные направления световой установки
            Console.WriteLine("\nAll Light Rig Direction Types:");
            foreach (LightRigDirectionType direction in Enum.GetValues(typeof(LightRigDirectionType)))
            {
                Console.WriteLine(direction.ToString());
            }

            // Сохраните книгу
            workbook.Save("LightRigDirectionTypeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


