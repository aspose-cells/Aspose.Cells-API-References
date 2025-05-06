---
title: MatrixEquationNode.IsHidePlaceholder
second_title: Aspose.Cells for .NET API Reference
description: MatrixEquationNode property. This attribute specifies the Hide Placeholders property on a matrix. When this property is on placeholders do not appear in the matrix.Default placeholders do appear such that the locations where text can be inserted are made visible
type: docs
url: /net/aspose.cells.drawing.equations/matrixequationnode/ishideplaceholder/
---
## MatrixEquationNode.IsHidePlaceholder property

This attribute specifies the Hide Placeholders property on a matrix. When this property is on, placeholders do not appear in the matrix.Default, placeholders do appear such that the locations where text can be inserted are made visible.

```csharp
public bool IsHidePlaceholder { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(true, matrixNode.IsHidePlaceholder);
[Test]
        public void Property_IsHidePlaceholder()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            //test get mathnode
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            MatrixEquationNode node = (MatrixEquationNode)mathNode.AddChild(EquationNodeType.Matrix);

            node.BaseJc = EquationVerticalJustificationType.Bottom;
            node.IsHidePlaceholder = true;

            //mr
            for (int i = 0; i &lt; 2; ++i)
            {
                EquationNode node1 = node.AddChild(EquationNodeType.MatrixRow);
                //col
                for (int j = 0; j &lt; 2; ++j)
                {
                    //e
                    EquationNode tmpNode2 = node1.AddChild(EquationNodeType.Base);
                    TextRunEquationNode tmpNode3 = (TextRunEquationNode)tmpNode2.AddChild(EquationNodeType.Text);
                    if (i==j)
                    {
                        tmpNode3.Text = &quot;1&quot;;
                    }
                }
            }

            string resultFile = Constants.destPath + &quot;MatrixEquationTest.xlsx&quot;;
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
            for (int i = 0; i &lt; 2; ++i)
            {
                EquationNode mrNode = matrixNode.GetChild(i);
                Assert.AreNotEqual(null, mrNode);
                Assert.AreEqual(EquationNodeType.MatrixRow, mrNode.EquationType);

                //col
                for (int j = 0; j &lt; 2; ++j)
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
                        Assert.AreEqual(&quot;1&quot;, TR.Text);
                    }

                }
            }
        }
```

### See Also

* class [MatrixEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


