---
title: "EquationNode.ParentNode"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство EquationNode. Указывает родительский узел текущего узла"
type: docs
url: /ru/net/aspose.cells.drawing.equations/equationnode/parentnode/
---
## EquationNode.ParentNode property

Указывает родительский узел текущего узла

```csharp
public EquationNode ParentNode { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodePropertyParentNodeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Создайте текстовое поле с уравнением
                TextBox textBox = worksheet.Shapes.AddTextBox(3, 0, 3, 0, 100, 200);
                EquationNode rootNode = textBox.GetEquationParagraph().GetChild(0);

                // Создайте дочерний узел
                EquationNode childNode = rootNode.AddChild(EquationNodeType.Sub);

                // Отобразите значения свойства ParentNode
                Console.WriteLine("Root node ParentNode: " + (rootNode.ParentNode == null ? "null" : "not null"));
                Console.WriteLine("Child node ParentNode: " + (childNode.ParentNode == null ? "null" : "not null"));

                // Проверьте отношение родитель‑дочерний
                if (childNode.ParentNode != null)
                {
                    Console.WriteLine("Child's parent is root: " + (childNode.ParentNode == rootNode));
                }

                // Продемонстрировать установку ParentNode (поскольку он читается и записывается)
                EquationNode newParent = EquationNode.CreateNode(EquationNodeType.Function, workbook, null);
                childNode.ParentNode = newParent;
                Console.WriteLine("After changing parent - Child's new parent: " + (childNode.ParentNode == newParent));

                workbook.Save("ParentNodeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


