---
title: "BoxEquationNode.Equals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод BoxEquationNode. Определить, равен ли текущий узел уравнения указанному узлу"
type: docs
url: /ru/net/aspose.cells.drawing.equations/boxequationnode/equals/
---
## BoxEquationNode.Equals method

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

    public class BoxEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте два объекта BoxEquationNode для сравнения
            // Поскольку у BoxEquationNode нет конструктора без параметров,
            // нам потребуется создавать их иначе. Предполагая, что мы можем получить их откуда‑то,
            // или создать их с некоторыми параметрами по умолчанию.
            // Для демонстрационных целей мы просто объявим их и присвоим null (хотя в реальном коде потребуется правильная инициализация)
            BoxEquationNode node1 = null;
            BoxEquationNode node2 = null;
            object objToCompare = node2;

            try
            {
                if (node1 != null && node2 != null)
                {
                    // Вызовите метод Equals с конкретными типами параметров (Object)
                    bool areEqual = node1.Equals(objToCompare);

                    // Отобразить результат
                    Console.WriteLine($"The BoxEquationNode objects are equal: {areEqual}");

                    // Добавить результат в лист
                    worksheet.Cells["A1"].PutValue("BoxEquationNode Equals Method Result:");
                    worksheet.Cells["B1"].PutValue(areEqual);
                }
                else
                {
                    Console.WriteLine("BoxEquationNode objects not properly initialized");
                    worksheet.Cells["A1"].PutValue("BoxEquationNode objects not properly initialized");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
                worksheet.Cells["A1"].PutValue("Error occurred:");
                worksheet.Cells["B1"].PutValue(ex.Message);
            }

            // Сохранить результат
            workbook.Save("BoxEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### См. также

* class [BoxEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


