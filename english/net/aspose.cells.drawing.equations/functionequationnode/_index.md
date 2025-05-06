---
title: Class FunctionEquationNode
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.Equations.FunctionEquationNode class. This class specifies the FunctionApply equation which consists of a function name and an argument acted upon. The types of the name and argument components are EquationNodeType.FunctionName and EquationNodeType.Base respectively
type: docs
url: /net/aspose.cells.drawing.equations/functionequationnode/
---
## FunctionEquationNode class

This class specifies the Function-Apply equation, which consists of a function name and an argument acted upon. The types of the name and argument components are 'EquationNodeType.FunctionName' and 'EquationNodeType.Base' respectively.

```csharp
public class FunctionEquationNode : EquationNode
```

## Properties

| Name | Description |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Get the equation type of the current node(Inherited from [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Returns the font of this object.(Inherited from [`FontSetting`](../../aspose.cells/fontsetting/).) |
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
| override [Equals](../../aspose.cells.drawing.equations/functionequationnode/equals/)(object) | Determine whether the current equation node is equal to the specified node |
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
// Called: FunctionEquationNode node = (FunctionEquationNode)mathNode.AddChild(EquationNodeType.Function);
[Test]
        public void Type_FunctionEquationNode()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            //test get mathnode
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            Assert.AreNotEqual(null, mathNode);

            //Add 
            string[] vals = new string[3] { &quot;Add&quot;, &quot;-2&quot;, &quot;x&quot; };
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

            string resultFile = Constants.destPath + &quot;FunctionEquationTest.xlsx&quot;;
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

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


