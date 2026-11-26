---
title: "GroupCharacterEquationNode.ChrType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство GroupCharacterEquationNode. Укажите комбинирующие символы по значению типа"
type: docs
url: /ru/net/aspose.cells.drawing.equations/groupcharacterequationnode/chrtype/
---
## GroupCharacterEquationNode.ChrType property

Укажите комбинирующие символы по значению типа.

```csharp
public EquationCombiningCharacterType ChrType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class GroupCharacterEquationNodePropertyChrTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить уравнение на первый лист
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Получить корневой узел уравнения
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Добавить узел группового символа
            GroupCharacterEquationNode groupNode = (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
            
            // Установить свойства группового символа
            groupNode.Position = EquationCharacterPositionType.Top;
            groupNode.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;

            // Добавить базовый текст
            EquationNode baseNode = groupNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "test";

            // Сохраните книгу
            workbook.Save("GroupCharacterEquationDemo.xlsx");

            // Проверьте сохранённый файл
            Workbook verifyWorkbook = new Workbook("GroupCharacterEquationDemo.xlsx");
            TextBox verifyTextBox = (TextBox)verifyWorkbook.Worksheets[0].Shapes[0];
            GroupCharacterEquationNode verifyNode = (GroupCharacterEquationNode)verifyTextBox.GetEquationParagraph()
                .GetChild(0).GetChild(0);

            Console.WriteLine("Group Character Type: " + verifyNode.ChrType);
            Console.WriteLine("Group Character: " + verifyNode.GroupChr);
            Console.WriteLine("Base Text: " + ((TextRunEquationNode)verifyNode.GetChild(0).GetChild(0)).Text);
        }
    }
}
```

### См. также

* enum [EquationCombiningCharacterType](../../equationcombiningcharactertype/)
* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


