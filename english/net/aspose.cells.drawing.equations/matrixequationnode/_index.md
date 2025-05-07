---
title: Class MatrixEquationNode
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.Equations.MatrixEquationNode class. This class specifies the Matrix equation consisting of one or more elements laid out in one or more rows and one or more columns
type: docs
url: /net/aspose.cells.drawing.equations/matrixequationnode/
---
## MatrixEquationNode class

This class specifies the Matrix equation, consisting of one or more elements laid out in one or more rows and one or more columns.

```csharp
public class MatrixEquationNode : EquationNode
```

## Properties

| Name | Description |
| --- | --- |
| [BaseJc](../../aspose.cells.drawing.equations/matrixequationnode/basejc/) { get; set; } | This attribute specifies the justification of the matrix. Text outside of the matrix can be aligned with the bottom, top, or center of a matrix function. Default, the matrix assumes center justification. |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Get the equation type of the current node(Inherited from [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Returns the font of this object.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [IsHidePlaceholder](../../aspose.cells.drawing.equations/matrixequationnode/ishideplaceholder/) { get; set; } | This attribute specifies the Hide Placeholders property on a matrix. When this property is on, placeholders do not appear in the matrix.Default, placeholders do appear such that the locations where text can be inserted are made visible. |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Gets the length of the characters.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Specifies the parent node of the current node(Inherited from [`EquationNode`](../equationnode/).) |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Gets the start index of the characters.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Returns the text options.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Represents the type of the node.(Inherited from [`EquationNode`](../equationnode/).) |

## Methods

| Name | Description |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | Inserts the specified node at the end of the current node's list of child nodes.(Inherited from [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | Insert a node of the specified type at the end of the child node list of the current node.(Inherited from [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/matrixequationnode/equals/)(object) | Determine whether the current equation node is equal to the specified node |
| [GetChild](../../aspose.cells.drawing.equations/equationnode/getchild/)(int) | Returns the node at the specified index among the children of the current node.(Inherited from [`EquationNode`](../equationnode/).) |
| [InsertAfter](../../aspose.cells.drawing.equations/equationnode/insertafter/)(EquationNodeType) | Inserts the specified node after the current node.(Inherited from [`EquationNode`](../equationnode/).) |
| [InsertBefore](../../aspose.cells.drawing.equations/equationnode/insertbefore/)(EquationNodeType) | Inserts the specified node before the current node.(Inherited from [`EquationNode`](../equationnode/).) |
| [InsertChild](../../aspose.cells.drawing.equations/equationnode/insertchild/)(int, EquationNodeType) | Inserts a node of the specified type at the specified index position in the current node's child node list.(Inherited from [`EquationNode`](../equationnode/).) |
| [Remove](../../aspose.cells.drawing.equations/equationnode/remove/)() | Removes itself from the parent.(Inherited from [`EquationNode`](../equationnode/).) |
| [RemoveAllChildren](../../aspose.cells.drawing.equations/equationnode/removeallchildren/)() | Removes all the child nodes of the current node.(Inherited from [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(EquationNode) | Removes the specified node from the current node's children.(Inherited from [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(int) | Removes the node at the specified index from the current node's children.(Inherited from [`EquationNode`](../equationnode/).) |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Sets the preset WordArt style.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ToLaTeX](../../aspose.cells.drawing.equations/equationnode/tolatex/)() | Convert this equtation to LaTeX expression.(Inherited from [`EquationNode`](../equationnode/).) |
| [ToMathML](../../aspose.cells.drawing.equations/equationnode/tomathml/)() | Convert this equtation to MathML expression.(Inherited from [`EquationNode`](../equationnode/).) |

### Examples

```csharp
// Called: MatrixEquationNode matrixNode = (MatrixEquationNode)mathNode2.GetChild(0);
[Test]
        public void Type_MatrixEquationNode()
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

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


