---
title: "SubSupEquationNode.Equals"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SubSupEquationNode. تحديد ما إذا كان عقدة المعادلة الحالية مساوية للعقدة المحددة"
type: docs
url: /ar/net/aspose.cells.drawing.equations/subsupequationnode/equals/
---
## SubSupEquationNode.Equals method

تحديد ما إذا كانت عقدة المعادلة الحالية مساوية للعقدة المحددة

```csharp
public override bool Equals(object obj)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | Object | العقدة المحددة |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Drawing;
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class SubSupEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            try
            {
                Workbook workbook = new Workbook();
                TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

                //اختبار الحصول على mathnode
                EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

                string[] vals = new string[] { "A", "B", "C" };
                int[] vs = null;
                EquationNode node = null;
                for (int i = 0; i < 4; i++)
                {
                    switch (i)
                    {
                        case 0:
                            node = mathNode.AddChild(EquationNodeType.Sub);
                            vs = new int[2] { 0, 1 };
                            break;
                        case 1:
                            node = mathNode.AddChild(EquationNodeType.Sup);
                            vs = new int[2] { 0, 2 };
                            break;
                        case 2:
                            node = mathNode.AddChild(EquationNodeType.SubSup);
                            vs = new int[3] { 0, 1, 2 };
                            break;
                        case 3:
                            node = mathNode.AddChild(EquationNodeType.PreSubSup);
                            vs = new int[3] { 1, 2, 0 };
                            break;
                    }

                    foreach (var v in vs)
                    {
                        switch (v)
                        {
                            case 0:
                                EquationNode e = node.AddChild(EquationNodeType.Base);
                                TextRunEquationNode TR = (TextRunEquationNode)(e.AddChild(EquationNodeType.Text));
                                TR.Text = vals[v];
                                break;
                            case 1:
                                EquationNode sub = node.AddChild(EquationNodeType.Subscript);
                                TR = (TextRunEquationNode)(sub.AddChild(EquationNodeType.Text));
                                TR.Text = vals[v];
                                break;
                            case 2:
                                EquationNode sup = node.AddChild(EquationNodeType.Superscript);
                                TR = (TextRunEquationNode)(sup.AddChild(EquationNodeType.Text));
                                TR.Text = vals[v];
                                break;
                        }
                    }
                }

                SubSupEquationNode node1 = (SubSupEquationNode)mathNode.GetChild(0);
                SubSupEquationNode node2 = (SubSupEquationNode)mathNode.GetChild(1);           
                

                // قارن العقد باستخدام طريقة Equals
                bool areEqual = node1.Equals((object)node2);
                
                // اعرض نتيجة المقارنة
                Console.WriteLine($"Are the nodes equal? {areEqual}");

                // قارن العقد باستخدام طريقة Equals
                areEqual = node1.Equals((object)node1);

                // اعرض نتيجة المقارنة
                Console.WriteLine($"Are the nodes equal? {areEqual}");

                // قارن مع نوع كائن مختلف
                object differentObject = new object();
                bool areEqualWithObject = node1.Equals(differentObject);
                Console.WriteLine($"Is node equal to a generic object? {areEqualWithObject}");

                workbook.Save("SubSupEquationNodeMethodEqualsWithObjectDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in Equals comparison: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SubSupEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


