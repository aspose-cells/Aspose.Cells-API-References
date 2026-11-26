---
title: "FractionEquationNode.Equals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FractionEquationNode. Определяет, равен ли текущий узел уравнения указанному узлу"
type: docs
url: /ru/net/aspose.cells.drawing.equations/fractionequationnode/equals/
---
## FractionEquationNode.Equals method

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

    public class FractionEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // Поскольку у FractionEquationNode нет конструктора без параметров,
                // Мы продемонстрируем Equals с объектами, которые, предположительно, приходят из других частей API
                // Для демонстрационных целей будем считать, что у нас есть два экземпляра для сравнения
                FractionEquationNode node1 = GetSampleFractionEquationNode(EquationFractionType.Bar);
                FractionEquationNode node2 = GetSampleFractionEquationNode(EquationFractionType.Skewed);

                // Сравните объекты, используя Equals
                bool areEqual = node1.Equals(node2);

                // Отобразите результат сравнения
                Console.WriteLine($"The FractionEquationNode instances are equal: {areEqual}");

                // Сравнить с null
                bool isNullEqual = node1.Equals(null);
                Console.WriteLine($"Comparison with null: {isNullEqual}");

                // Сравните с самим собой
                bool isSelfEqual = node1.Equals(node1);
                Console.WriteLine($"Comparison with self: {isSelfEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in Equals demonstration: {ex.Message}");
            }
        }

        // Вспомогательный метод для имитации получения экземпляров FractionEquationNode
        // (В реальном использовании эти объекты будут получены из API)
        private static FractionEquationNode GetSampleFractionEquationNode(EquationFractionType fractionType)
        {
            // Это просто заполнитель — на самом деле вы бы получили их из API
            // Например: worksheet.Equations.AddFractionEquationNode() или аналогично
            return null; // Actual implementation would depend on API
        }
    }
}
```

### См. также

* class [FractionEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


