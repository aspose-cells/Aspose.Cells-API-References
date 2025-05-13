---
title: MatrixEquationNode.BaseJc
second_title: Aspose.Cells for .NET API Reference
description: MatrixEquationNode property. This attribute specifies the justification of the matrix. Text outside of the matrix can be aligned with the bottom top or center of a matrix function. Default the matrix assumes center justification
type: docs
url: /net/aspose.cells.drawing.equations/matrixequationnode/basejc/
---
## MatrixEquationNode.BaseJc property

This attribute specifies the justification of the matrix. Text outside of the matrix can be aligned with the bottom, top, or center of a matrix function. Default, the matrix assumes center justification.

```csharp
public EquationVerticalJustificationType BaseJc { get; set; }
```

### Examples

```csharp
// Called: node.BaseJc = EquationVerticalJustificationType.Bottom;
public void MatrixEquationNode_Property_BaseJc()
{
    Workbook workbook = new Workbook();
    TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

    //test get mathnode
    EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
    MatrixEquationNode node = (MatrixEquationNode)mathNode.AddChild(EquationNodeType.Matrix);

    node.BaseJc = EquationVerticalJustificationType.Bottom;
    node.IsHidePlaceholder = true;

    //mr
    for (int i = 0; i < 2; ++i)
    {
        EquationNode node1 = node.AddChild(EquationNodeType.MatrixRow);
        //col
        for (int j = 0; j < 2; ++j)
        {
            //e
            EquationNode tmpNode2 = node1.AddChild(EquationNodeType.Base);
            TextRunEquationNode tmpNode3 = (TextRunEquationNode)tmpNode2.AddChild(EquationNodeType.Text);
            if (i==j)
            {
                tmpNode3.Text = "1";
            }
        }
    }

    string resultFile = Constants.destPath + "MatrixEquationTest.xlsx";
    workbook.Save(resultFile);
    Workbook workbook2 = new Workbook(resultFile);

    TextBox textBoxRead = (TextBox)workbook2.Worksheets[0].Shapes[0];
    EquationNode mathNode2 = textBoxRead.GetEquationParagraph().GetChild(0);
    Assert.AreNotEqual(null, mathNode2);

    MatrixEquationNode matrixNode = (MatrixEquationNode)mathNode2.GetChild(0);
    Assert.AreNotEqual(null, matrixNode);
    Assert.AreEqual(EquationNodeType.Matrix, matrixNode.EquationType);
    Assert.AreEqual(EquationVerticalJustificationType.Bottom, matrixNode.BaseJc);
    Assert.AreEqual(true, matrixNode.IsHidePlaceholder);

    //mr
    for (int i = 0; i < 2; ++i)
    {
        EquationNode mrNode = matrixNode.GetChild(i);
        Assert.AreNotEqual(null, mrNode);
        Assert.AreEqual(EquationNodeType.MatrixRow, mrNode.EquationType);

        //col
        for (int j = 0; j < 2; ++j)
        {
            //e
            EquationNode baseNode = mrNode.GetChild(j);
            Assert.AreNotEqual(null, baseNode);
            Assert.AreEqual(EquationNodeType.Base, baseNode.EquationType);

            TextRunEquationNode TR = (TextRunEquationNode)baseNode.GetChild(0);
            Assert.AreNotEqual(null, TR);
            Assert.AreEqual(EquationNodeType.Text, TR.EquationType);

            if (i == j)
            {
                Assert.AreEqual("1", TR.Text);
            }

        }
    }
}
```

### See Also

* enum [EquationVerticalJustificationType](../../equationverticaljustificationtype/)
* class [MatrixEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


