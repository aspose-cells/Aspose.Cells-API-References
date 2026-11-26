---
title: "Перечисление EquationVerticalJustificationType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.Equations.EquationVerticalJustificationType. Это указывает значение вертикального выравнивания уравнений по умолчанию в документе"
type: docs
url: /ru/net/aspose.cells.drawing.equations/equationverticaljustificationtype/
---
## EquationVerticalJustificationType enumeration

Это определяет вертикальное выравнивание уравнений в документе по умолчанию.

```csharp
public enum EquationVerticalJustificationType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Top | `0` | верх |
| Center | `1` | центр |
| Bottom | `2` | низ |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationVerticalJustificationTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте форму уравнения на первый лист
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Получить абзац уравнения и добавить узел матрицы
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            MatrixEquationNode matrixNode = (MatrixEquationNode)mathNode.AddChild(EquationNodeType.Matrix);

            // Установить свойства матрицы
            matrixNode.BaseJc = EquationVerticalJustificationType.Bottom;
            matrixNode.IsHidePlaceholder = true;

            // Добавить строки и столбцы матрицы
            for (int i = 0; i < 2; i++)
            {
                EquationNode rowNode = matrixNode.AddChild(EquationNodeType.MatrixRow);
                
                for (int j = 0; j < 2; j++)
                {
                    EquationNode baseNode = rowNode.AddChild(EquationNodeType.Base);
                    TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
                    textNode.Text = (i == j) ? "1" : "0";
                }
            }

            // Сохраните книгу
            string outputPath = "EquationVerticalJustificationDemo.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("File saved with vertical justification demo: " + outputPath);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


