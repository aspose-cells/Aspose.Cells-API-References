---
title: "EquationNode.ToLaTeX"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод EquationNode. Преобразовать это уравнение в выражение LaTeX"
type: docs
url: /ru/net/aspose.cells.drawing.equations/equationnode/tolatex/
---
## EquationNode.ToLaTeX method

Преобразовать это уравнение в выражение LaTeX.

```csharp
public string ToLaTeX()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodToLaTeXDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать форму для размещения уравнения
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 0, 0);

            // Получить узел уравнения
            var equationNode = shape.GetEquationParagraph();

            // Создать простое уравнение дроби
            var fractionNode = equationNode.AddChild(EquationNodeType.Fraction);
            var numerator = fractionNode.AddChild(EquationNodeType.Numerator);
            var numeratorText = numerator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            numeratorText.Text = "1";
            var denominator = fractionNode.AddChild(EquationNodeType.Denominator);
            var denominatorText = denominator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            denominatorText.Text = "2";

            try
            {
                // Вызвать метод ToLaTeX
                string latexExpression = equationNode.ToLaTeX();
                
                // Отобразить результат
                Console.WriteLine("LaTeX expression: " + latexExpression);
                
                // Добавить вывод LaTeX в ячейку
                worksheet.Cells["A1"].PutValue("LaTeX Output:");
                worksheet.Cells["B1"].PutValue(latexExpression);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ToLaTeX method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("EquationToLaTeXDemo.xlsx");
        }
    }
}
```

### См. также

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


