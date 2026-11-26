---
title: "BarEquationNode.Equals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод BarEquationNode. Определить, равен ли текущий узел уравнения указанному узлу"
type: docs
url: /ru/net/aspose.cells.drawing.equations/barequationnode/equals/
---
## BarEquationNode.Equals method

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

    public class BarEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать два экземпляра BarEquationNode для сравнения
            // Примечание: Фактическое создание BarEquationNode будет зависеть от фабричных методов API
            // Для демонстрации будем считать, что эти экземпляры правильно инициализированы
            BarEquationNode node1 = GetBarEquationNode(EquationCharacterPositionType.Top);
            BarEquationNode node2 = GetBarEquationNode(EquationCharacterPositionType.Top);
            BarEquationNode node3 = GetBarEquationNode(EquationCharacterPositionType.Bottom);

            try
            {
                // Сравнить node1 с node2 (должны быть равны)
                bool result1 = node1.Equals(node2);
                Console.WriteLine($"Comparing node1 with node2: {result1}");

                // Сравнить node1 с node3 (не должны быть равны)
                bool result2 = node1.Equals(node3);
                Console.WriteLine($"Comparing node1 with node3: {result2}");

                // Сравнить node1 с null
                bool result3 = node1.Equals(null);
                Console.WriteLine($"Comparing node1 with null: {result3}");

                // Сравнить node1 с объектом другого типа
                bool result4 = node1.Equals("string object");
                Console.WriteLine($"Comparing node1 with string: {result4}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("BarEquationNodeEqualsDemo.xlsx");
        }

        // Вспомогательный метод для демонстрации получения BarEquationNode
        // В реальном использовании вы бы использовали правильный метод API для их создания
        private static BarEquationNode GetBarEquationNode(EquationCharacterPositionType position)
        {
            // Это всего лишь заполнитель — реальная реализация будет зависеть от API
            // Например, он может быть создан через родительский объект или фабричный метод
            return null; // Replace with actual creation code
        }
    }
}
```

### См. также

* class [BarEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


