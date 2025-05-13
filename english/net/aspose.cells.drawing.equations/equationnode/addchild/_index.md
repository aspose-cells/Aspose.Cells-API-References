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
// Called: TextRunEquationNode supTR = (TextRunEquationNode)(sup.AddChild(EquationNodeType.Text));
public void EquationNode_Method_AddChild()
{
    Workbook workbook = new Workbook();
    TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

    //test get mathnode
    EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
    Assert.AreNotEqual(null, mathNode);

    //Add 
    string[] vals = new string[3] { "Add", "-2", "x" };
    FunctionEquationNode node = (FunctionEquationNode)mathNode.AddChild(EquationNodeType.Function);

    EquationNode subNode1 = node.AddChild(EquationNodeType.FunctionName);
    EquationNode supf = subNode1.AddChild(EquationNodeType.Sup);

    EquationNode e = supf.AddChild(EquationNodeType.Base);
    TextRunEquationNode eTR = (TextRunEquationNode)(e.AddChild(EquationNodeType.Text));
    eTR.Text = vals[0];

    EquationNode sup = supf.AddChild(EquationNodeType.Superscript);
    TextRunEquationNode supTR = (TextRunEquationNode)(sup.AddChild(EquationNodeType.Text));
    supTR.Text = vals[1];

    EquationNode subNode2 = node.AddChild(EquationNodeType.Base);
    TextRunEquationNode TR = (TextRunEquationNode)(subNode2.AddChild(EquationNodeType.Text));
    TR.Text = vals[2];

    string resultFile = Constants.destPath + "FunctionEquationTest.xlsx";
    workbook.Save(resultFile);
    Workbook workbook2 = new Workbook(resultFile);

    TextBox textBoxRead = (TextBox)workbook2.Worksheets[0].Shapes[0];
    EquationNode mathNode2 = textBoxRead.GetEquationParagraph().GetChild(0);
    Assert.AreNotEqual(null, mathNode2);


    //test 1
    FunctionEquationNode function = (FunctionEquationNode)mathNode2.GetChild(0);
    Assert.AreNotEqual(null, function);
    Assert.AreEqual(EquationNodeType.Function, function.EquationType);

    EquationNode fName = function.GetChild(0);
    Assert.AreNotEqual(null, fName);
    Assert.AreEqual(EquationNodeType.FunctionName, fName.EquationType);

    EquationNode SuperE = fName.GetChild(0);
    Assert.AreNotEqual(null, SuperE);
    Assert.AreEqual(EquationNodeType.Sup, SuperE.EquationType);

    EquationNode eBase = SuperE.GetChild(0);
    Assert.AreNotEqual(null, eBase);
    Assert.AreEqual(EquationNodeType.Base, eBase.EquationType);
    TR = (TextRunEquationNode)eBase.GetChild(0);
    Assert.AreNotEqual(null, TR);
    Assert.AreEqual(EquationNodeType.Text, TR.EquationType);
    Assert.AreEqual(vals[0], TR.Text);

    EquationNode supr = SuperE.GetChild(1);
    Assert.AreNotEqual(null, supr);
    Assert.AreEqual(EquationNodeType.Superscript, supr.EquationType);
    TR = (TextRunEquationNode)supr.GetChild(0);
    Assert.AreNotEqual(null, TR);
    Assert.AreEqual(EquationNodeType.Text, TR.EquationType);
    Assert.AreEqual(vals[1], TR.Text);

    EquationNode nodeTmp1 = function.GetChild(1);
    Assert.AreNotEqual(null, nodeTmp1);
    Assert.AreEqual(EquationNodeType.Base, nodeTmp1.EquationType);
    TR = (TextRunEquationNode)nodeTmp1.GetChild(0);
    Assert.AreNotEqual(null, TR);
    Assert.AreEqual(EquationNodeType.Text, TR.EquationType);
    Assert.AreEqual(vals[2], TR.Text);
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


