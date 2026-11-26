---
title: "EquationNode.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство EquationNode. Представляет тип узла"
type: docs
url: /ru/net/aspose.cells.drawing.equations/equationnode/type/
---
## EquationNode.Type property

Представляет тип узла.

```csharp
public override TextNodeType Type { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class EquationNodePropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать форму уравнения
            var shape = worksheet.Shapes.AddEquation(0, 0, 300, 100, 0, 0);
            var equationRoot = shape.GetEquationParagraph();

            // Создайте разные типы узлов уравнения
            var fractionNode = equationRoot.AddChild(EquationNodeType.Fraction);
            var textNode = equationRoot.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            textNode.Text = "Sample Text";

            // Отобразите свойство Type для разных узлов
            Console.WriteLine($"Root equation node type: {equationRoot.Type}");
            Console.WriteLine($"Fraction node type: {fractionNode.Type}");
            Console.WriteLine($"Text node type: {textNode.Type}");

            // Создайте сложную структуру уравнения
            var numerator = fractionNode.AddChild(EquationNodeType.Numerator);
            var numeratorText = numerator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            numeratorText.Text = "Numerator";

            var denominator = fractionNode.AddChild(EquationNodeType.Denominator);
            var denominatorText = denominator.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            denominatorText.Text = "Denominator";

            // Проверьте типы дочерних узлов
            Console.WriteLine($"Numerator node type: {numerator.Type}");
            Console.WriteLine($"Numerator text node type: {numeratorText.Type}");
            Console.WriteLine($"Denominator node type: {denominator.Type}");

            // Продемонстрируйте, как Type влияет на поведение узла
            if (textNode.Type == TextNodeType.TextRun)
            {
                Console.WriteLine("Text node is a TextRun type - can contain text content");
            }

            if (fractionNode.Type == TextNodeType.Equation)
            {
                Console.WriteLine("Fraction node is an Equation type - can contain child nodes");
            }

            // Сохранить результат
            workbook.Save("EquationNodePropertyTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [TextNodeType](../../../aspose.cells.drawing.texts/textnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


