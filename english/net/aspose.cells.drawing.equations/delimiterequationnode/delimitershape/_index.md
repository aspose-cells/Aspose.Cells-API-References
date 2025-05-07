---
title: DelimiterEquationNode.DelimiterShape
second_title: Aspose.Cells for .NET API Reference
description: DelimiterEquationNode property. Specifies the shape of delimiters in the delimiter object
type: docs
url: /net/aspose.cells.drawing.equations/delimiterequationnode/delimitershape/
---
## DelimiterEquationNode.DelimiterShape property

Specifies the shape of delimiters in the delimiter object.

```csharp
public EquationDelimiterShapeType DelimiterShape { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(EquationDelimiterShapeType.Centered, node2.DelimiterShape);
[Test]
        public void Property_DelimiterShape()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            //test get mathnode
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            Assert.AreNotEqual(null, mathNode);

            //add 1
            DelimiterEquationNode node = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);

            //add 2
            node = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
            node.DelimiterShape = EquationDelimiterShapeType.Match;
            node.NaryGrow = false;
            node.SeparatorChar = "!";
            node.BeginChar = "#";
            node.EndChar = "*";

            EquationNode e = node.AddChild(EquationNodeType.Base);

            FractionEquationNode Fra = (FractionEquationNode)e.AddChild(EquationNodeType.Fraction);

            EquationComponentNode numerator = (EquationComponentNode)Fra.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode TR = (TextRunEquationNode)(numerator.AddChild(EquationNodeType.Text));
            TR.Text = "A";

            EquationComponentNode denominator = (EquationComponentNode)Fra.AddChild(EquationNodeType.Denominator);
            TR = (TextRunEquationNode)(denominator.AddChild(EquationNodeType.Text));
            TR.Text = "B";

            EquationNode e2 = node.AddChild(EquationNodeType.Base);
            TextRunEquationNode tr2 = (TextRunEquationNode)e2.AddChild(EquationNodeType.Text);
            tr2.Text = "a";

            string resultFile = Constants.destPath + "BracketEquationTest.xlsx";
            workbook.Save(resultFile);
            Workbook workbook2 = new Workbook(resultFile);

            TextBox textBoxRead = (TextBox)workbook2.Worksheets[0].Shapes[0];
            EquationNode mathNode2 = textBoxRead.GetEquationParagraph().GetChild(0);
            Assert.AreNotEqual(null, mathNode2);

            //test 1
            DelimiterEquationNode node2 = (DelimiterEquationNode)mathNode2.GetChild(0);
            Assert.AreNotEqual(null, node2);
            Assert.AreEqual(EquationNodeType.Delimiter, node2.EquationType);

            Assert.AreEqual("(", node2.BeginChar);
            Assert.AreEqual(")", node2.EndChar);
            Assert.AreEqual(false, node2.NaryGrow);
            Assert.AreEqual("|", node2.SeparatorChar);
            Assert.AreEqual(EquationDelimiterShapeType.Centered, node2.DelimiterShape);

            //test 2
            node2 = (DelimiterEquationNode)mathNode2.GetChild(1);
            Assert.AreNotEqual(null, node2);
            Assert.AreEqual(EquationNodeType.Delimiter, node2.EquationType);

            Assert.AreEqual("#", node2.BeginChar);
            Assert.AreEqual("*", node2.EndChar);
            Assert.AreEqual(false, node2.NaryGrow);
            Assert.AreEqual("!", node2.SeparatorChar);
            Assert.AreEqual(EquationDelimiterShapeType.Match, node2.DelimiterShape);

        }
```

### See Also

* enum [EquationDelimiterShapeType](../../equationdelimitershapetype/)
* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


