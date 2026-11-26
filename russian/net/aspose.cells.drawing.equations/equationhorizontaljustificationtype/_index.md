---
title: "Перечисление EquationHorizontalJustificationType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.Equations.EquationHorizontalJustificationType enum. Указывает стандартное горизонтальное выравнивание уравнений в документе"
type: docs
url: /ru/net/aspose.cells.drawing.equations/equationhorizontaljustificationtype/
---
## EquationHorizontalJustificationType enumeration

Это определяет горизонтальное выравнивание уравнений в документе по умолчанию.

```csharp
public enum EquationHorizontalJustificationType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Center | `0` | По центру |
| CenterGroup | `1` | По центру как группа |
| Left | `2` | Выравнено по левому краю |
| Right | `3` | Выравнено по правому краю |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationsClassEquationHorizontalJustificationTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Добавьте форму уравнения на лист
                TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

                // Получить абзац уравнения
                EquationNodeParagraph equationNode = (EquationNodeParagraph)textBox.GetEquationParagraph();

                // Продемонстрировать различные типы горизонтального выравнивания
                equationNode.Justification = EquationHorizontalJustificationType.Center;
                Console.WriteLine("Current Justification: " + equationNode.Justification);

                equationNode.Justification = EquationHorizontalJustificationType.Left;
                Console.WriteLine("Current Justification: " + equationNode.Justification);

                equationNode.Justification = EquationHorizontalJustificationType.Right;
                Console.WriteLine("Current Justification: " + equationNode.Justification);

                // Сохраните книгу
                workbook.Save("EquationHorizontalJustificationTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with EquationHorizontalJustificationType: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


