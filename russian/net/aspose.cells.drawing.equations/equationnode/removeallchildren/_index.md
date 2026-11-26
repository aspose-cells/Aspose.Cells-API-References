---
title: "EquationNode.RemoveAllChildren"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод EquationNode. Удаляет все дочерние узлы текущего узла"
type: docs
url: /ru/net/aspose.cells.drawing.equations/equationnode/removeallchildren/
---
## EquationNode.RemoveAllChildren method

Удаляет все дочерние узлы текущего узла.

```csharp
public void RemoveAllChildren()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodRemoveAllChildrenDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать форму для размещения уравнения
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);

            // Получить узел уравнения
            var equationNode = ((TextBox)shape).GetEquationParagraph();

            // Добавьте несколько дочерних узлов к уравнению
            var fractionNode = equationNode.AddChild(EquationNodeType.Fraction);
            var numerator = fractionNode.AddChild(EquationNodeType.Numerator);
            numerator.AddChild(EquationNodeType.Text).ToLaTeX(); // Access text content through ToLaTeX or ToMathML
            var denominator = fractionNode.AddChild(EquationNodeType.Denominator);
            denominator.AddChild(EquationNodeType.Text).ToLaTeX(); // Access text content through ToLaTeX or ToMathML

            Console.WriteLine($"Equation before RemoveAllChildren: {equationNode.ToMathML()}");

            try
            {
                // Вызовите метод RemoveAllChildren
                equationNode.RemoveAllChildren();

                Console.WriteLine("Method executed successfully");
                Console.WriteLine($"Equation after RemoveAllChildren: {equationNode.ToMathML()}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAllChildren method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("EquationNodeMethodRemoveAllChildrenDemo.xlsx");
        }
    }
}
```

### См. также

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


