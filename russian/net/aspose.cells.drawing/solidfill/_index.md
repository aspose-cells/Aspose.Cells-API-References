---
title: "Класс SolidFill"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.SolidFill. Инкапсулирует объект, представляющий формат сплошной заливки"
type: docs
url: /ru/net/aspose.cells.drawing/solidfill/
---
## SolidFill class

Инкапсулирует объект, представляющий формат сплошной заливки.

```csharp
public class SolidFill : Fill
```

## Свойства

| Имя | Описание |
| --- | --- |
| [CellsColor](../../aspose.cells.drawing/solidfill/cellscolor/) { get; set; } | Получает и задает объект [`CellsColor`](./cellscolor/). |
| [Color](../../aspose.cells.drawing/solidfill/color/) { get; set; } | Получает или задает цвет. |
| [Transparency](../../aspose.cells.drawing/solidfill/transparency/) { get; set; } | Возвращает или задает степень прозрачности области значением от 0.0 (непрозрачный) до 1.0 (прозрачный). |

## Методы

| Имя | Описание |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/solidfill/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/solidfill/gethashcode/)() | Получает хеш‑код. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using System;
    using System.Drawing;
    using Aspose.Cells;
    using Aspose.Cells.Drawing;

    public class DrawingClassSolidFillDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            try
            {
                // Добавить простую прямоугольную форму на лист
                Shape rect = sheet.Shapes.AddRectangle(2, 0, 2, 0, 150, 100);

                // Настроить форму для использования сплошной заливки
                rect.Fill.FillType = FillType.Solid;

                // Получить объект SolidFill
                SolidFill solidFill = rect.Fill.SolidFill;

                // Установить свойства сплошной заливки
                solidFill.Color = Color.CornflowerBlue;   // System.Drawing.Color
                solidFill.Transparency = 0.25;            // 0 = opaque, 1 = fully transparent

                // Получить доступ к свойству CellsColor (чтение/запись)
                CellsColor cellsColor = solidFill.CellsColor;
                if (cellsColor != null)
                {
                    Console.WriteLine("CellsColor object is available.");
                }
                else
                {
                    Console.WriteLine("CellsColor is null (default).");
                }

                Console.WriteLine($"SolidFill created with Color={solidFill.Color.Name}, Transparency={solidFill.Transparency}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SolidFill: {ex.Message}");
            }

            // Сохраните рабочую книгу, чтобы проверить внешний вид фигуры
            workbook.Save("DrawingClassSolidFillDemo.xlsx");
        }
    }
}
```

### См. также

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


