---
title: "EquationNode.ToMathML"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод EquationNode. Преобразует это уравнение в выражение MathML"
type: docs
url: /ru/net/aspose.cells.drawing.equations/equationnode/tomathml/
---
## EquationNode.ToMathML method

Преобразовать это уравнение в выражение MathML.

```csharp
public string ToMathML()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodToMathMLDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте форму уравнения — добавлен параметр ширины (300) и параметр высоты (100)
            var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 300, 100);
            var equation = shape.GetEquationParagraph();

            // Постройте простое уравнение: (a+b)^2 = a^2 + 2ab + b^2
            var equationNode = equation.AddChild(EquationNodeType.Text);
            var textNode = equationNode as TextRunEquationNode;
            textNode.Text = "(";

            var variableA = equation.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            variableA.Text = "a";

            var plus = equation.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            plus.Text = "+";

            var variableB = equation.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            variableB.Text = "b";

            var closeParen = equation.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            closeParen.Text = ")";

            var superscript = equation.AddChild(EquationNodeType.Superscript);
            var baseNode = superscript.AddChild(EquationNodeType.Base);
            var baseText = baseNode.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            baseText.Text = "2";

            try
            {
                // Преобразуйте уравнение в MathML
                string mathML = equation.ToMathML();

                // Выведите MathML в консоль
                Console.WriteLine("MathML Output:");
                Console.WriteLine(mathML);

                // Запишите MathML в ячейку
                worksheet.Cells["A1"].PutValue("MathML Representation:");
                worksheet.Cells["A2"].PutValue(mathML);
                // Изменено с worksheet.Cells.AutoFitColumns() на:
                worksheet.AutoFitColumns();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error converting to MathML: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("EquationToMathMLDemo.xlsx");
        }
    }
}
```

### См. также

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


