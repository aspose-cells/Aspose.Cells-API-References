---
title: ShapeCollection.AddEquation
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Add an equation object to the worksheet
type: docs
url: /net/aspose.cells.drawing/shapecollection/addequation/
---
## ShapeCollection.AddEquation method

Add an equation object to the worksheet.

```csharp
public TextBox AddEquation(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| topRow | Int32 | The top row index. |
| top | Int32 | The vertical offset its top row, in unit of pixel. |
| leftColumn | Int32 | The left column index. |
| left | Int32 | The horizontal offset from its left column, in unit of pixel. |
| height | Int32 | The height of equation, in unit of pixel. |
| width | Int32 | The width of equation, in unit of pixel. |

### Examples

```csharp
// Called: TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);
public void ShapeCollection_Method_AddEquation()
{
    Workbook workbook = new Workbook();
    TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

    //test get mathnode
    EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
    Assert.AreNotEqual(null, mathNode);

    //test insert Fraction
    FractionEquationNode node = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
    node.FractionType = EquationFractionType.Skewed;

    string str1 = "A";
    EquationComponentNode numerator = (EquationComponentNode)node.AddChild(EquationNodeType.Numerator);
    TextRunEquationNode TR = (TextRunEquationNode)(numerator.AddChild(EquationNodeType.Text));
    TR.Text = str1;

    string str2 = "B";
    EquationComponentNode denominator = (EquationComponentNode)node.AddChild(EquationNodeType.Denominator);
    TR = (TextRunEquationNode)(denominator.AddChild(EquationNodeType.Text));
    TR.Text = str2;

    workbook.Save(Constants.destPath + "FractionEquationTest.xlsx");
    workbook = new Workbook(Constants.destPath + "FractionEquationTest.xlsx");

    TextBox textBoxRead = (TextBox)workbook.Worksheets[0].Shapes[0];
    EquationNode mathNode2 = textBoxRead.GetEquationParagraph().GetChild(0);
    Assert.AreNotEqual(null, mathNode2);

    FractionEquationNode node2 = (FractionEquationNode)mathNode2.GetChild(0);
    Assert.AreNotEqual(null, node2);
    Assert.AreEqual(EquationFractionType.Skewed, node2.FractionType);

    EquationComponentNode numerator2 = (EquationComponentNode)node2.GetChild(0);
    Assert.AreNotEqual(null, numerator2);
    Assert.AreEqual(EquationNodeType.Numerator, numerator2.EquationType);

    EquationComponentNode denominator2 = (EquationComponentNode)node2.GetChild(1);
    Assert.AreNotEqual(null, denominator2);
    Assert.AreEqual(EquationNodeType.Denominator, denominator2.EquationType);

    TextRunEquationNode TR1 = (TextRunEquationNode)numerator2.GetChild(0);
    Assert.AreNotEqual(null, TR1);
    Assert.AreEqual(str1, TR1.Text);

    TextRunEquationNode TR2 = (TextRunEquationNode)denominator2.GetChild(0);
    Assert.AreNotEqual(null, TR2);
    Assert.AreEqual(str2, TR2.Text);

}
```

### See Also

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


