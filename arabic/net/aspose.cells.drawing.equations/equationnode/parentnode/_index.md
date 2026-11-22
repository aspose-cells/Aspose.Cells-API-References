---
title: "EquationNode.ParentNode"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية EquationNode. تحدد العقدة الأصلية للعقدة الحالية"
type: docs
url: /ar/net/aspose.cells.drawing.equations/equationnode/parentnode/
---
## EquationNode.ParentNode property

يحدد العقدة الأم للعقدة الحالية

```csharp
public EquationNode ParentNode { get; set; }
```

### أمثلة

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
                // إنشاء مربع نص مع معادلة
                TextBox textBox = worksheet.Shapes.AddTextBox(3, 0, 3, 0, 100, 200);
                EquationNode rootNode = textBox.GetEquationParagraph().GetChild(0);

                // إنشاء عقدة فرعية
                EquationNode childNode = rootNode.AddChild(EquationNodeType.Sub);

                // عرض قيم خاصية ParentNode
                Console.WriteLine("Root node ParentNode: " + (rootNode.ParentNode == null ? "null" : "not null"));
                Console.WriteLine("Child node ParentNode: " + (childNode.ParentNode == null ? "null" : "not null"));

                // التحقق من علاقة الأصل بالابن
                if (childNode.ParentNode != null)
                {
                    Console.WriteLine("Child's parent is root: " + (childNode.ParentNode == rootNode));
                }

                // عرض تعيين ParentNode (نظرًا لأنه قابل للقراءة والكتابة)
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

### انظر أيضًا

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


