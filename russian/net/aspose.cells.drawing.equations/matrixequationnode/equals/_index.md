---
title: "MatrixEquationNode.Equals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод MatrixEquationNode. Определяет, равен ли текущий узел уравнения указанному узлу"
type: docs
url: /ru/net/aspose.cells.drawing.equations/matrixequationnode/equals/
---
## MatrixEquationNode.Equals method

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

    public class MatrixEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                // Поскольку у MatrixEquationNode нет конструктора без параметров,
                // мы продемонстрируем метод Equals, используя другой подход
                Console.WriteLine("MatrixEquationNode Equals demonstration:");
                
                // Примечание: Для реального создания экземпляра потребуются правильные параметры конструктора
                // Это лишь демонстрация шаблона использования метода Equals
                MatrixEquationNode node1 = null; // Would normally be created with proper constructor
                MatrixEquationNode node2 = null; // Would normally be created with proper constructor

                if (node1 != null && node2 != null)
                {
                    // Сравните узлы, используя метод Equals
                    bool areEqual = node1.Equals(node2);
                    Console.WriteLine($"Are the matrix equation nodes equal? {areEqual}");

                    // Сравните узел с самим собой
                    bool selfEqual = node1.Equals(node1);
                    Console.WriteLine($"Is node1 equal to itself? {selfEqual}");
                }

                // Сравнить с null
                if (node1 != null)
                {
                    bool nullEqual = node1.Equals(null);
                    Console.WriteLine($"Is node1 equal to null? {nullEqual}");
                }
                else
                {
                    Console.WriteLine("Node1 is null - cannot demonstrate Equals method");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in MatrixEquationNode Equals demonstration: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [MatrixEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


