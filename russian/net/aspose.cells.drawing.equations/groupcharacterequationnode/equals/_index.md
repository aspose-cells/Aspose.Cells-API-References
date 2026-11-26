---
title: "GroupCharacterEquationNode.Equals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GroupCharacterEquationNode. Определить, равен ли текущий узел уравнения указанному узлу"
type: docs
url: /ru/net/aspose.cells.drawing.equations/groupcharacterequationnode/equals/
---
## GroupCharacterEquationNode.Equals method

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

    public class GroupCharacterEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте два экземпляра GroupCharacterEquationNode для сравнения
            // Поскольку у GroupCharacterEquationNode нет конструктора без параметров,
            // нам потребуется создать их через ShapeCollection листа
            var shape1 = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
            var node1 = (GroupCharacterEquationNode)shape1.GetEquationParagraph().AddChild(EquationNodeType.GroupChr);
            node1.GroupChr = "⏟";
            node1.ChrType = EquationCombiningCharacterType.BottomCurlyBracket;
            node1.Position = EquationCharacterPositionType.Bottom;
            node1.VertJc = EquationCharacterPositionType.Bottom;

            var shape2 = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
            var node2 = (GroupCharacterEquationNode)shape2.GetEquationParagraph().AddChild(EquationNodeType.GroupChr);
            node2.GroupChr = "⏟";
            node2.ChrType = EquationCombiningCharacterType.BottomCurlyBracket;
            node2.Position = EquationCharacterPositionType.Bottom;
            node2.VertJc = EquationCharacterPositionType.Bottom;

            try
            {
                // Вызовите метод Equals с параметром Object.
                bool areEqual = node1.Equals((Object)node2);

                // Отобразите результат сравнения
                Console.WriteLine($"The two GroupCharacterEquationNode instances are equal: {areEqual}");

                // Добавить результат в лист
                worksheet.Cells["A1"].PutValue("GroupCharacterEquationNode Equals Comparison Result:");
                worksheet.Cells["A2"].PutValue(areEqual);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("GroupCharacterEquationNodeEqualsDemo.xlsx");
        }
    }
}
```

### См. также

* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


