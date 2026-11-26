---
title: "Перечисление EquationFractionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.Equations.EquationFractionType. Это определяет стиль отображения черты дроби"
type: docs
url: /ru/net/aspose.cells.drawing.equations/equationfractiontype/
---
## EquationFractionType enumeration

Это определяет стиль отображения черты дроби.

```csharp
public enum EquationFractionType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Bar | `0` | Это указывает, что числитель находится сверху, а знаменатель снизу, разделённые чертой посередине. |
| NoBar | `1` | Это указывает, что числитель находится сверху, а знаменатель снизу, но они не разделены чертой посередине. |
| Linear | `2` | Это указывает, что числитель слева, а знаменатель справа, разделённые символом '/' между ними. |
| Skewed | `3` | Это указывает, что числитель в верхнем левом углу, а знаменатель в нижнем правом, разделённые символом "/". |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationFractionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить форму уравнения
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Получите математический узел и добавьте дробь
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            FractionEquationNode fractionNode = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
            fractionNode.FractionType = EquationFractionType.Skewed;

            // Добавить числитель
            EquationComponentNode numerator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode numeratorText = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            numeratorText.Text = "A";

            // Добавить знаменатель
            EquationComponentNode denominator = (EquationComponentNode)fractionNode.AddChild(EquationNodeType.Denominator);
            TextRunEquationNode denominatorText = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            denominatorText.Text = "B";

            // Сохранить и проверить
            workbook.Save("EquationFractionTypeDemo.xlsx");
            
            Console.WriteLine("Equation with skewed fraction created successfully.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


