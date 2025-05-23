---
title: RadicalEquationNode.IsDegHide
second_title: Aspose.Cells for .NET API Reference
description: RadicalEquationNode property. Whether to hide the degree of radicals
type: docs
url: /net/aspose.cells.drawing.equations/radicalequationnode/isdeghide/
---
## RadicalEquationNode.IsDegHide property

Whether to hide the degree of radicals.

```csharp
public bool IsDegHide { get; set; }
```

### Examples

```csharp
// Called: node.IsDegHide = true;
public void RadicalEquationNode_Property_IsDegHide()
{
    Workbook workbook = new Workbook();
    TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

    //test get mathnode
    EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
    Assert.AreNotEqual(null, mathNode);

    RadicalEquationNode node = (RadicalEquationNode)mathNode.AddChild(EquationNodeType.Radical);
    node.IsDegHide = true;
    //IsDegHide = true,deg invalid,do not write to file
    EquationNode deg = node.AddChild(EquationNodeType.Degree);
    TextRunEquationNode tr = (TextRunEquationNode)deg.AddChild(EquationNodeType.Text);
    tr.Text = "5";

    EquationNode e = node.AddChild(EquationNodeType.Base);
    TextRunEquationNode tr2 = (TextRunEquationNode)e.AddChild(EquationNodeType.Text);
    tr2.Text = "a";

    workbook.Save(Constants.destPath + "RadicalEquationTest.xlsx");
    workbook = new Workbook(Constants.destPath + "RadicalEquationTest.xlsx");

    TextBox textBoxRead = (TextBox)workbook.Worksheets[0].Shapes[0];
    EquationNode mathNode2 = textBoxRead.GetEquationParagraph().GetChild(0);
    Assert.AreNotEqual(null, mathNode2);

    RadicalEquationNode node2 = (RadicalEquationNode)mathNode2.GetChild(0);
    Assert.AreNotEqual(null, node2);
    Assert.AreEqual(true, node2.IsDegHide);

    EquationComponentNode deg2 = (EquationComponentNode)node2.GetChild(0);
    Assert.AreNotEqual(null, deg2);
    Assert.AreEqual(EquationNodeType.Degree, deg2.EquationType);

    EquationComponentNode e2 = (EquationComponentNode)node2.GetChild(1);
    Assert.AreNotEqual(null, e2);
    Assert.AreEqual(EquationNodeType.Base, e2.EquationType);

    TextRunEquationNode TR1 = (TextRunEquationNode)deg2.GetChild(0);
    Assert.AreEqual(null, TR1);

    TextRunEquationNode TR2 = (TextRunEquationNode)e2.GetChild(0);
    Assert.AreNotEqual(null, TR2);
    Assert.AreEqual("a", TR2.Text);
}
```

### See Also

* class [RadicalEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


