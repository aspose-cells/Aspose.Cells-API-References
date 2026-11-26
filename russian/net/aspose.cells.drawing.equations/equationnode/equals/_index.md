---
title: "EquationNode.Equals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод EquationNode. Определяет, равен ли текущий узел уравнения указанному узлу"
type: docs
url: /ru/net/aspose.cells.drawing.equations/equationnode/equals/
---
## EquationNode.Equals method

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
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте два узла уравнения для сравнения
            EquationNode node1 = EquationNode.CreateNode(EquationNodeType.Function, workbook, null);
            EquationNode node2 = EquationNode.CreateNode(EquationNodeType.Function, workbook, null);

            try
            {
                // Вызовите метод Equals с параметром Object
                bool areEqual = node1.Equals((object)node2);

                Console.WriteLine($"Are the equation nodes equal? {areEqual}");

                // Изменить node2, чтобы они стали различными
                node2.AddChild(EquationNodeType.Base);

                areEqual = node1.Equals((object)node2);
                Console.WriteLine($"After modification, are they equal? {areEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            workbook.Save("EquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### См. также

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


