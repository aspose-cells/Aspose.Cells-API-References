---
title: "NaryEquationNode.NaryOperatorType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство NaryEquationNode. nary‑оператор, например"
type: docs
url: /ru/net/aspose.cells.drawing.equations/naryequationnode/naryoperatortype/
---
## NaryEquationNode.NaryOperatorType property

n-арный оператор, например "∑"

```csharp
public EquationMathematicalOperatorType NaryOperatorType { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class NaryEquationNodePropertyNaryOperatorTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать форму для размещения уравнения
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 200, 50);

            // Получите доступ к уравнению и добавьте узел nary‑оператора
            var equation = shape.GetEquationParagraph();
            var naryNode = equation.AddChild(EquationNodeType.NaryEquation);

            // Приведите к NaryEquationNode, чтобы получить доступ к NaryOperatorType
            var naryEquationNode = (NaryEquationNode)naryNode;

            // Отобразите текущий NaryOperatorType (значение по умолчанию)
            Console.WriteLine("Current NaryOperatorType: " + naryEquationNode.NaryOperatorType);

            // Установите оператор суммы (∑)
            naryEquationNode.NaryOperatorType = EquationMathematicalOperatorType.NarySummation;

            // Добавьте основание (операнд) и пределы, чтобы продемонстрировать оператор
            var baseNode = naryEquationNode.AddChild(EquationNodeType.Base);
            var textNode1 = baseNode.AddChild(EquationNodeType.Text);
            textNode1.ToLaTeX(); // This would be where you'd set the text content if the API allowed
            var limitNode = naryEquationNode.AddChild(EquationNodeType.Limit);
            var textNode2 = limitNode.AddChild(EquationNodeType.Text);
            textNode2.ToLaTeX(); // This would be where you'd set the text content if the API allowed
            var textNode3 = baseNode.AddChild(EquationNodeType.Text);
            textNode3.ToLaTeX(); // This would be where you'd set the text content if the API allowed

            // Установите оператор, чтобы он рос вместе с содержимым
            naryEquationNode.NaryGrow = true;

            // Измените на оператор произведения (∏) и покажите разницу
            naryEquationNode.NaryOperatorType = EquationMathematicalOperatorType.NaryProduct;

            // Сохраните книгу
            workbook.Save("NaryOperatorTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [EquationMathematicalOperatorType](../../equationmathematicaloperatortype/)
* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


