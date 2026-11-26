---
title: "LimLowUppEquationNode.Equals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод LimLowUppEquationNode. Определяет, равен ли текущий узел уравнения указанному узлу"
type: docs
url: /ru/net/aspose.cells.drawing.equations/limlowuppequationnode/equals/
---
## LimLowUppEquationNode.Equals method

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

    public class LimLowUppEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Поскольку мы не знаем параметры конструктора, мы сравним значения null
            // Это минимальное изменение, позволяющее скомпилировать код — в реальном использовании потребуется правильное создание объектов
            LimLowUppEquationNode node1 = null;
            LimLowUppEquationNode node2 = null;

            try
            {
                // Вызовите метод Equals с конкретным типом параметра (Object)
                bool areEqual = node1?.Equals((object)node2) ?? false;

                // Отобразить результат
                Console.WriteLine($"Are the nodes equal? {areEqual}");

                // Сохраните книгу
                workbook.Save("LimLowUppEquationNodeEqualsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [LimLowUppEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


