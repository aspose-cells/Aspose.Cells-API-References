---
title: "NaryEquationNode.NaryGrow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство NaryEquationNode. Этот атрибут определяет свойство роста nary‑операторов на уровне документа. Когда отключено, nary‑операторы, такие как интегралы и суммы, не увеличиваются, чтобы соответствовать высоте их операнда. Когда включено, nary‑оператор растёт вертикально, чтобы соответствовать высоте своего операнда."
type: docs
url: /ru/net/aspose.cells.drawing.equations/naryequationnode/narygrow/
---
## NaryEquationNode.NaryGrow property

Этот атрибут задает свойство роста n-арных операторов на уровне документа. Когда отключено, n-арные операторы, такие как интегралы и суммы, не увеличиваются, чтобы соответствовать высоте их операнда. Когда включено, n-арный оператор растет вертикально, чтобы соответствовать высоте операнда.

```csharp
public bool NaryGrow { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class NaryEquationNodePropertyNaryGrowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить форму уравнения
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            // Получить узел уравнения
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Создайте узел nary‑оператора с установленным свойством NaryGrow в значение true
            NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            naryNode.NaryOperator = "∑";
            naryNode.NaryGrow = true; // This is the key property we're demonstrating
            
            // Добавьте нижний индекс (необязательно)
            EquationNode sub = naryNode.AddChild(EquationNodeType.Subscript);
            TextRunEquationNode subText = (TextRunEquationNode)sub.AddChild(EquationNodeType.Text);
            subText.Text = "i=1";
            
            // Добавьте верхний индекс (необязательно)
            EquationNode sup = naryNode.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode supText = (TextRunEquationNode)sup.AddChild(EquationNodeType.Text);
            supText.Text = "n";
            
            // Добавьте основание (обязательно)
            EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x_i";
            
            // Сохраните книгу
            workbook.Save("NaryGrowDemo.xlsx");
            
            Console.WriteLine("Equation with NaryGrow property created successfully.");
        }
    }
}
```

### См. также

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


