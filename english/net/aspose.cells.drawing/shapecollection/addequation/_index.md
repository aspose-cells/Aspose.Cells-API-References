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
[Test]
        public void Method_Int32_()
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

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


