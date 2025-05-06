---
title: EquationNode.AddChild
second_title: Aspose.Cells for .NET API Reference
description: EquationNode method. Insert a node of the specified type at the end of the child node list of the current node
type: docs
url: /net/aspose.cells.drawing.equations/equationnode/addchild/
---
## AddChild(EquationNodeType) {#addchild}

Insert a node of the specified type at the end of the child node list of the current node.

```csharp
public EquationNode AddChild(EquationNodeType equationType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| equationType | EquationNodeType | Types of Equation Nodes |

### Return Value

If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.

### Examples

```csharp
// Called: TextRunEquationNode tr = (TextRunEquationNode)deg.AddChild(EquationNodeType.Text);
[Test]
        public void Method_EquationNodeType_()
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
            tr.Text = &quot;5&quot;;

            EquationNode e = node.AddChild(EquationNodeType.Base);
            TextRunEquationNode tr2 = (TextRunEquationNode)e.AddChild(EquationNodeType.Text);
            tr2.Text = &quot;a&quot;;

            workbook.Save(Constants.destPath + &quot;RadicalEquationTest.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;RadicalEquationTest.xlsx&quot;);

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
            Assert.AreEqual(&quot;a&quot;, TR2.Text);
        }
```

### See Also

* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)

---

## AddChild(EquationNode) {#addchild_1}

Inserts the specified node at the end of the current node's list of child nodes.

```csharp
public void AddChild(EquationNode node)
```

| Parameter | Type | Description |
| --- | --- | --- |
| node | EquationNode | The specified node |

### See Also

* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


