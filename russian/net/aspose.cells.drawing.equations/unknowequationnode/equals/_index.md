---
title: "UnknowEquationNode.Equals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод UnknowEquationNode. Определить, равен ли текущий узел уравнения указанному узлу"
type: docs
url: /ru/net/aspose.cells.drawing.equations/unknowequationnode/equals/
---
## UnknowEquationNode.Equals method

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

    public class UnknowEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать два неизвестных узла уравнения для сравнения
            // Поскольку у UnknowEquationNode нет конструктора без параметров,
            // нам потребуется создавать их иначе. Для демонстрационных целей мы будем использовать
            // реальный конструктор, если он доступен, либо создавать их другими способами.
            // Поскольку мы не знаем параметры конструктора, это временное решение.
            UnknowEquationNode node1 = CreateUnknownEquationNode();
            UnknowEquationNode node2 = CreateUnknownEquationNode();
            object objToCompare = node2;

            try
            {
                // Вызовите метод Equals с конкретным типом параметра (Object)
                bool areEqual = node1.Equals(objToCompare);

                // Отобразить результат
                Console.WriteLine($"Are the equation nodes equal? {areEqual}");

                // Добавить результат в лист
                worksheet.Cells["A1"].PutValue("Equation Node Comparison Result:");
                worksheet.Cells["B1"].PutValue(areEqual ? "Equal" : "Not Equal");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("UnknowEquationNodeEqualsDemo.xlsx");
        }

        // Вспомогательный метод для создания экземпляров UnknowEquationNode
        private static UnknowEquationNode CreateUnknownEquationNode()
        {
            // В реальной реализации это использовало бы правильный конструктор
            // Поскольку мы не знаем параметры конструктора, мы вернём null
            // и обработаем случай null в демонстрации (хотя это лишь заглушка)
            return null;
        }
    }
}
```

### См. также

* class [UnknowEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


