---
title: "ArrayEquationNode.Equals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ArrayEquationNode. Определить, равен ли текущий узел уравнения указанному узлу"
type: docs
url: /ru/net/aspose.cells.drawing.equations/arrayequationnode/equals/
---
## ArrayEquationNode.Equals method

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

    public class ArrayEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте два узла уравнения массива
            ArrayEquationNode arrayEquation1 = (ArrayEquationNode)EquationNode.CreateNode(EquationNodeType.ArrayEquation, workbook, null);
            ArrayEquationNode arrayEquation2 = (ArrayEquationNode)EquationNode.CreateNode(EquationNodeType.ArrayEquation, workbook, null);

            // Добавьте дочерние узлы, чтобы сделать их различными
            EquationNode child1 = EquationNode.CreateNode(EquationNodeType.Text, workbook, arrayEquation1);
            // Используйте ToLaTeX() или ToMathML() вместо свойства Value
            arrayEquation1.AddChild(child1);

            EquationNode child2 = EquationNode.CreateNode(EquationNodeType.Text, workbook, arrayEquation2);
            arrayEquation2.AddChild(child2);

            try
            {
                // Вызовите метод Equals с разными объектами
                bool result1 = arrayEquation1.Equals(arrayEquation2);
                Console.WriteLine($"Comparing different array equations: {result1}");

                // Вызовите Equals с тем же объектом
                bool result2 = arrayEquation1.Equals(arrayEquation1);
                Console.WriteLine($"Comparing same array equation: {result2}");

                // Вызовите Equals с null
                bool result4 = arrayEquation1.Equals(null);
                Console.WriteLine($"Comparing with null: {result4}");
                
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("ArrayEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### См. также

* class [ArrayEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


