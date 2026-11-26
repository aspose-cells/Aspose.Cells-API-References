---
title: "MathematicalEquationNode.Equals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод MathematicalEquationNode. Определить, равен ли текущий узел уравнения указанному узлу"
type: docs
url: /ru/net/aspose.cells.drawing.equations/mathematicalequationnode/equals/
---
## MathematicalEquationNode.Equals method

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
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class MathematicalEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // Создайте два экземпляра MathematicalEquationNode для сравнения
                // Поскольку у MathematicalEquationNode нет конструктора без параметров,
                // нам потребуется передать null или соответствующие параметры
                MathematicalEquationNode node1 = null;
                MathematicalEquationNode node2 = null;
                
                // Сравните узлы, используя метод Equals
                bool areEqual = node1?.Equals((object)node2) ?? false;
                
                // Отобразите результат сравнения
                Console.WriteLine($"Nodes are equal: {areEqual}");
                
                // Сравните с объектом другого типа
                object differentObject = new object();
                bool areEqualWithObject = node1?.Equals(differentObject) ?? false;
                Console.WriteLine($"Node equals generic object: {areEqualWithObject}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in Equals comparison: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [MathematicalEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


