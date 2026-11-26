---
title: "NaryEquationNode.Equals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод NaryEquationNode. Определить, равен ли текущий узел уравнения указанному узлу"
type: docs
url: /ru/net/aspose.cells.drawing.equations/naryequationnode/equals/
---
## NaryEquationNode.Equals method

Определить, равен ли текущий узел уравнения указанному узлу

```csharp
public override bool Equals(object obj)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | Object | Указанный узел |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class NaryEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать форму для размещения уравнения
            var shape1 = worksheet.Shapes.AddEquation(0, 0, 200, 50, 200, 50);
            var equation1 = shape1.GetEquationParagraph();
            var naryNode1 = equation1.AddChild(EquationNodeType.NaryEquation);
            var naryEquationNode1 = (NaryEquationNode)naryNode1;
            naryEquationNode1.NaryOperatorType = EquationMathematicalOperatorType.NarySummation;

            // Создать вторую идентичную форму
            var shape2 = worksheet.Shapes.AddEquation(0, 100, 200, 50, 200, 50);
            var equation2 = shape2.GetEquationParagraph();
            var naryNode2 = equation2.AddChild(EquationNodeType.NaryEquation);
            var naryEquationNode2 = (NaryEquationNode)naryNode2;
            naryEquationNode2.NaryOperatorType = EquationMathematicalOperatorType.NarySummation;

            // Создать третью различную форму
            var shape3 = worksheet.Shapes.AddEquation(0, 200, 200, 50, 200, 50);
            var equation3 = shape3.GetEquationParagraph();
            var naryNode3 = equation3.AddChild(EquationNodeType.NaryEquation);
            var naryEquationNode3 = (NaryEquationNode)naryNode3;
            naryEquationNode3.NaryOperatorType = EquationMathematicalOperatorType.NaryProduct;

            try
            {
                // Сравнить идентичные узлы
                bool result1 = naryEquationNode1.Equals(naryEquationNode2);
                Console.WriteLine($"Comparing identical nodes: {result1}");

                // Сравнить разные узлы
                bool result2 = naryEquationNode1.Equals(naryEquationNode3);
                Console.WriteLine($"Comparing different nodes: {result2}");

                // Сравнить с null
                bool result3 = naryEquationNode1.Equals(null);
                Console.WriteLine($"Comparing with null: {result3}");

                // Сравнить с объектом другого типа
                bool result4 = naryEquationNode1.Equals("string object");
                Console.WriteLine($"Comparing with different type: {result4}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("NaryEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### См. также

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


