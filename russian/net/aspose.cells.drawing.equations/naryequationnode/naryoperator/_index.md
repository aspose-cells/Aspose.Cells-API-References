---
title: "NaryEquationNode.NaryOperator"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство NaryEquationNode. nary‑оператор, например. Настоятельно рекомендуется использовать атрибут NaryOperatorType для установки nary‑оператора. Используйте эту настройку свойства, если не можете найти нужный символ в известном типе"
type: docs
url: /ru/net/aspose.cells.drawing.equations/naryequationnode/naryoperator/
---
## NaryEquationNode.NaryOperator property

n-арный оператор, например "∑". Настоятельно рекомендуется использовать атрибут NaryOperatorType для установки n-арного оператора. Используйте эту настройку свойства, если не можете найти нужный символ в известном типе.

```csharp
public string NaryOperator { get; set; }
```

### Примечания

Следует отметить, что это свойство принимает только один символ, и если передано несколько символов, принимается только первый.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class NaryEquationNodePropertyNaryOperatorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму уравнения
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Получить узел уравнения
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // Создать узел nary‑оператора
            NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            
            // Установить свойства nary‑оператора
            naryNode.NaryOperator = "\u2211"; // Summation symbol
            naryNode.NaryGrow = true;

            // Добавьте нижний индекс (необязательно)
            EquationNode subscript = naryNode.AddChild(EquationNodeType.Subscript);
            TextRunEquationNode subscriptText = (TextRunEquationNode)subscript.AddChild(EquationNodeType.Text);
            subscriptText.Text = "i=1";

            // Добавьте верхний индекс (необязательно)
            EquationNode superscript = naryNode.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode superscriptText = (TextRunEquationNode)superscript.AddChild(EquationNodeType.Text);
            superscriptText.Text = "n";

            // Добавить базовое выражение
            EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x_i";

            // Сохраните книгу
            workbook.Save("NaryOperatorDemo.xlsx");

            Console.WriteLine("Nary operator equation created successfully.");
        }
    }
}
```

### См. также

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


