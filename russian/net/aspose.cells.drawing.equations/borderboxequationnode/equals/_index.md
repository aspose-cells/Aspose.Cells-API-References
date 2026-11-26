---
title: "BorderBoxEquationNode.Equals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод BorderBoxEquationNode. Определить, равен ли текущий узел уравнения указанному узлу"
type: docs
url: /ru/net/aspose.cells.drawing.equations/borderboxequationnode/equals/
---
## BorderBoxEquationNode.Equals method

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

    public class BorderBoxEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // Создайте два экземпляра BorderBoxEquationNode для сравнения
                // Поскольку у BorderBoxEquationNode нет конструктора без параметров,
                // мы будем использовать конструктор базового класса (предполагая, что у EquationNode он может быть)
                BorderBoxEquationNode node1 = (BorderBoxEquationNode)Activator.CreateInstance(typeof(BorderBoxEquationNode));
                BorderBoxEquationNode node2 = (BorderBoxEquationNode)Activator.CreateInstance(typeof(BorderBoxEquationNode));
                
                // Сравните узлы, используя метод Equals
                bool areEqual = node1.Equals((object)node2);
                
                // Отобразите результат сравнения
                Console.WriteLine($"The nodes are equal: {areEqual}");
                
                // Сравните с объектом другого типа
                object differentObject = new object();
                bool areEqualWithDifferentType = node1.Equals(differentObject);
                Console.WriteLine($"Comparison with different type: {areEqualWithDifferentType}");
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

* class [BorderBoxEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


