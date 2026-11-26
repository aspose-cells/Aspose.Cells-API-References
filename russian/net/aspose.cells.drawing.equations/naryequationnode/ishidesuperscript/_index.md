---
title: "NaryEquationNode.IsHideSuperscript"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство NaryEquationNode. Отображать ли верхний предел"
type: docs
url: /ru/net/aspose.cells.drawing.equations/naryequationnode/ishidesuperscript/
---
## NaryEquationNode.IsHideSuperscript property

Отображать верхнюю границу

```csharp
public bool IsHideSuperscript { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class NaryEquationNodePropertyIsHideSuperscriptDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Создать узел nary equation с скрытым верхним индексом
            NaryEquationNode node = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            node.NaryOperator = "∫";
            node.IsHideSuperscript = true; // Demonstrating the IsHideSuperscript property
            
            // Добавить базовый компонент
            EquationNode baseNode = node.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x";
            
            // Добавить верхний индекс (будет скрыт из‑за IsHideSuperscript = true)
            EquationNode supNode = node.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode supText = (TextRunEquationNode)supNode.AddChild(EquationNodeType.Text);
            supText.Text = "2";

            // Сохранить и перезагрузить для проверки, что верхний индекс скрыт
            workbook.Save("NaryEquationDemo.xlsx");
            workbook = new Workbook("NaryEquationDemo.xlsx");
            
            // Проверить сохранённое уравнение
            TextBox savedTextBox = (TextBox)workbook.Worksheets[0].Shapes[0];
            EquationNode savedMathNode = savedTextBox.GetEquationParagraph().GetChild(0);
            NaryEquationNode savedNode = (NaryEquationNode)savedMathNode.GetChild(0);
            
            Console.WriteLine("Nary Operator: " + savedNode.NaryOperator);
            Console.WriteLine("IsHideSuperscript: " + savedNode.IsHideSuperscript);
            Console.WriteLine("Superscript exists: " + (savedNode.GetChild(1).GetChild(0) != null));
        }
    }
}
```

### См. также

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


