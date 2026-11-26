---
title: "FunctionEquationNode.Equals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FunctionEquationNode. Определить, равен ли текущий узел уравнения указанному узлу"
type: docs
url: /ru/net/aspose.cells.drawing.equations/functionequationnode/equals/
---
## FunctionEquationNode.Equals method

Определить, равен ли текущий узел уравнения указанному узлу

```csharp
public override bool Equals(object obj)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | Object | Указанный узел |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class FunctionEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму TextBox для размещения уравнения
            TextBox textBox = worksheet.Shapes.AddTextBox(3, 0, 3, 0, 200, 100);

            // Получить корневой узел уравнения TextBox
            EquationNode rootNode = textBox.GetEquationParagraph().GetChild(0);

            // Создать первый узел функции уравнения
            FunctionEquationNode funcNode1 = (FunctionEquationNode)rootNode.AddChild(EquationNodeType.Function);
            // (Опционально) Добавить минимальное содержимое, чтобы узел был корректным
            EquationNode funcName1 = funcNode1.AddChild(EquationNodeType.FunctionName);
            TextRunEquationNode nameText1 = (TextRunEquationNode)funcName1.AddChild(EquationNodeType.Text);
            nameText1.Text = "Sin";

            // Создать второй узел функции уравнения
            FunctionEquationNode funcNode2 = (FunctionEquationNode)rootNode.AddChild(EquationNodeType.Function);
            EquationNode funcName2 = funcNode2.AddChild(EquationNodeType.FunctionName);
            TextRunEquationNode nameText2 = (TextRunEquationNode)funcName2.AddChild(EquationNodeType.Text);
            nameText2.Text = "Cos";

            try
            {
                // Сравнить два узла функции с помощью Equals(Object)
                bool areEqual = funcNode1.Equals((object)funcNode2);
                Console.WriteLine($"funcNode1.Equals(funcNode2) returned: {areEqual}");

                // Сравнить узел с самим собой
                bool selfEqual = funcNode1.Equals((object)funcNode1);
                Console.WriteLine($"funcNode1.Equals(funcNode1) returned: {selfEqual}");

                // Сохранить книгу (визуальные изменения не требуются для этой демонстрации)
                workbook.Save("FunctionEquationNodeEqualsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during Equals demonstration: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [FunctionEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


