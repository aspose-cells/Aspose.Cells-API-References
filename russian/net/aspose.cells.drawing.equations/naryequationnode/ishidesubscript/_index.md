---
title: "NaryEquationNode.IsHideSubscript"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство NaryEquationNode. Определяет, отображать ли нижнюю границу"
type: docs
url: /ru/net/aspose.cells.drawing.equations/naryequationnode/ishidesubscript/
---
## NaryEquationNode.IsHideSubscript property

Отображать нижнюю границу

```csharp
public bool IsHideSubscript { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class NaryEquationNodePropertyIsHideSubscriptDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Создать узел Nary equation с скрытым нижним индексом
            NaryEquationNode node = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            node.NaryOperator = "∫";
            node.IsHideSubscript = true; // Hide subscript
            node.IsHideSuperscript = false; // Show superscript

            // Добавить нижний индекс (будет скрыт)
            EquationNode sub = node.AddChild(EquationNodeType.Subscript);
            TextRunEquationNode subText = (TextRunEquationNode)(sub.AddChild(EquationNodeType.Text));
            subText.Text = "1";

            // Добавить верхний индекс (будет видим)
            EquationNode sup = node.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode supText = (TextRunEquationNode)(sup.AddChild(EquationNodeType.Text));
            supText.Text = "5";

            // Добавить основание
            EquationNode e = node.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)(e.AddChild(EquationNodeType.Text));
            baseText.Text = "C";

            // Сохранить и проверить
            workbook.Save("NaryEquationDemo.xlsx");
            
            // Перезагрузить для проверки свойств
            Workbook loadedWorkbook = new Workbook("NaryEquationDemo.xlsx");
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            EquationNode loadedMathNode = loadedTextBox.GetEquationParagraph().GetChild(0);
            NaryEquationNode loadedNode = (NaryEquationNode)loadedMathNode.GetChild(0);
            
            Console.WriteLine("Nary Operator: " + loadedNode.NaryOperator);
            Console.WriteLine("IsHideSubscript: " + loadedNode.IsHideSubscript);
            Console.WriteLine("IsHideSuperscript: " + loadedNode.IsHideSuperscript);
        }
    }
}
```

### См. также

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


