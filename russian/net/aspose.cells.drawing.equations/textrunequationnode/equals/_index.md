---
title: "TextRunEquationNode.Equals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод TextRunEquationNode. Определить, равен ли текущий узел уравнения указанному узлу"
type: docs
url: /ru/net/aspose.cells.drawing.equations/textrunequationnode/equals/
---
## TextRunEquationNode.Equals method

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

    public class TextRunEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Для демонстрационных целей мы используем null и просто показываем логику сравнения
            // поскольку мы не можем создавать экземпляры TextRunEquationNode напрямую
            TextRunEquationNode node1 = null;
            TextRunEquationNode node2 = null;
            TextRunEquationNode node3 = null;

            try
            {
                // Эта часть оставлена, чтобы показать, как будет вызываться Equals
                // В реальном сценарии эти узлы будут правильно инициализированы
                if (node1 != null && node2 != null && node3 != null)
                {
                    // Сравнить node1 с node2 (одинаковое содержимое)
                    bool result1 = node1.Equals((object)node2);
                    Console.WriteLine($"Comparing nodes with same text 'x': {result1}");

                    // Сравнить node1 с node3 (разное содержимое)
                    bool result2 = node1.Equals((object)node3);
                    Console.WriteLine($"Comparing nodes with different text ('x' vs 'y'): {result2}");

                    // Сравнить с null
                    bool result3 = node1.Equals(null);
                    Console.WriteLine($"Comparing with null: {result3}");

                    // Сравнить с объектом другого типа
                    bool result4 = node1.Equals("string object");
                    Console.WriteLine($"Comparing with different type: {result4}");
                }
                else
                {
                    Console.WriteLine("Node instances not available - this is just a compilation demo");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Сохранить книгу (хотя Equals не изменяет таблицу)
            workbook.Save("TextRunEquationNodeEqualsDemo.xlsx");
        }

        // Удалён вспомогательный метод, поскольку мы не можем правильно создавать экземпляры TextRunEquationNode
    }
}
```

### См. также

* class [TextRunEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


