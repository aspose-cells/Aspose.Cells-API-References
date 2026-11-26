---
title: "GroupCharacterEquationNode.GroupChr"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство GroupCharacterEquationNode. Указывает символ по умолчанию U23DF. Настоятельно рекомендуется использовать атрибут ChrType для установки акцентного символа. Используйте эту настройку свойства, если не можете найти нужный символ в известном типе."
type: docs
url: /ru/net/aspose.cells.drawing.equations/groupcharacterequationnode/groupchr/
---
## GroupCharacterEquationNode.GroupChr property

Указывает символ (по умолчанию U+23DF). Настоятельно рекомендуется использовать атрибут ChrType для установки символа надстрочного знака. Используйте эту настройку свойства, если не можете найти нужный символ в известном типе.

```csharp
public string GroupChr { get; set; }
```

### Примечания

Следует отметить, что это свойство принимает только один символ, и если передано несколько символов, принимается только первый.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class GroupCharacterEquationNodePropertyGroupChrDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить уравнение на первый лист
            TextBox textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // Получить корневой узел уравнения
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Создать узел группового символа с двойной стрелкой вправо
            GroupCharacterEquationNode groupNode = 
                (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
            groupNode.Position = EquationCharacterPositionType.Top;
            groupNode.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;

            // Добавить базовый текст к групповому символу
            EquationNode baseNode = groupNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = 
                (TextRunEquationNode)(baseNode.AddChild(EquationNodeType.Text));
            textNode.Text = "abc";

            // Продемонстрировать использование свойства GroupChr
            Console.WriteLine("Group Character: " + groupNode.GroupChr); // Should output "⇒"

            // Сохраните книгу
            workbook.Save("GroupCharacterEquationDemo.xlsx");
        }
    }
}
```

### См. также

* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


