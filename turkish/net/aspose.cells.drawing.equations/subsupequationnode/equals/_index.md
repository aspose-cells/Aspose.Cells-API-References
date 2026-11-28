---
title: "SubSupEquationNode.Equals"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SubSupEquationNode yöntemi. Mevcut denklem düğümünün belirtilen düğüme eşit olup olmadığını belirleyin"
type: docs
url: /tr/net/aspose.cells.drawing.equations/subsupequationnode/equals/
---
## SubSupEquationNode.Equals method

Geçerli denklem düğümünün belirtilen düğüme eşit olup olmadığını belirle

```csharp
public override bool Equals(object obj)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | Object | Belirtilen düğüm |

### Örnekler

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

                //test al mathnode
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
                

                // Düğümleri Equals yöntemiyle karşılaştırın
                bool areEqual = node1.Equals((object)node2);
                
                // Karşılaştırma sonucunu gösterin
                Console.WriteLine($"Are the nodes equal? {areEqual}");

                // Düğümleri Equals yöntemiyle karşılaştırın
                areEqual = node1.Equals((object)node1);

                // Karşılaştırma sonucunu gösterin
                Console.WriteLine($"Are the nodes equal? {areEqual}");

                // Farklı bir nesne türüyle karşılaştırın
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

### Ayrıca Bakınız

* class [SubSupEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


