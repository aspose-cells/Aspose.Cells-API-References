---
title: "Перечисление FormatSetType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.FormatSetType. Тип набора формата заливки"
type: docs
url: /ru/net/aspose.cells.drawing/formatsettype/
---
## FormatSetType enumeration

Тип набора формата заливки.

```csharp
public enum FormatSetType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Без заливки. |
| IsGradientSet | `1` | Градиентный формат заливки. |
| IsTextureSet | `2` | Текстурный формат заливки. |
| IsPatternSet | `3` | Шаблонный формат заливки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassFormatSetTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Добавьте фигуру, чтобы продемонстрировать формат заливки
                Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 200);
                FillFormat fillFormat = shape.Fill;

                // Отобразить начальный тип заливки
                Console.WriteLine("Initial fill type: " + fillFormat.Type);

                // Продемонстрировать значения перечисления FormatSetType
                Console.WriteLine("FormatSetType.None: " + (int)FormatSetType.None);
                Console.WriteLine("FormatSetType.IsGradientSet: " + (int)FormatSetType.IsGradientSet);
                Console.WriteLine("FormatSetType.IsTextureSet: " + (int)FormatSetType.IsTextureSet);
                Console.WriteLine("FormatSetType.IsPatternSet: " + (int)FormatSetType.IsPatternSet);

                // Применить различные типы заливки с использованием FormatSetType
                fillFormat.Type = (FillType)FormatSetType.IsGradientSet;
                Console.WriteLine("After setting gradient: " + fillFormat.Type);

                fillFormat.Type = (FillType)FormatSetType.IsPatternSet;
                Console.WriteLine("After setting pattern: " + fillFormat.Type);

                // Сохраните книгу
                workbook.Save("FormatSetTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with FormatSetType: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


