---
title: "الفئة SubSupEquationNode"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.Equations.SubSupEquationNode. تحدد هذه الفئة معادلة يمكن أن تكون في المرتبة العلوية (superscript) أو السفلية (subscript) اختياريًا. هناك أربعة أشكال رئيسية لهذه المعادلة: superscript و subscript و superscript و subscript، حيث يتم وضع superscript و subscript إلى يسار القاعدة و superscript و subscript إلى يمين القاعدة"
type: docs
url: /ar/net/aspose.cells.drawing.equations/subsupequationnode/
---
## SubSupEquationNode class

هذه الفئة تحدد معادلة يمكن أن تكون اختيارياً مرتفعة أو منخفضة. هناك أربع صيغ رئيسية لهذه المعادلة: مرتفعة، منخفضة، مرتفعة ومنخفضة موضوعة إلى يسار القاعدة، مرتفعة ومنخفضة موضوعة إلى يمين القاعدة.

```csharp
public class SubSupEquationNode : EquationNode
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | احصل على نوع المعادلة للعقدة الحالية (موروث من [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | يعيد الخط لهذا الكائن. (موروث من [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | يحصل على طول الأحرف. (موروث من [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | يحدد العقدة الأب للعقدة الحالية (موروث من [`EquationNode`](../equationnode/).) |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | يحصل على الفهرس الابتدائي للأحرف. (موروث من [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | يعيد خيارات النص. (موروث من [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | يمثل نوع العقدة (موروث من [`EquationNode`](../equationnode/).) |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | يدرج العقدة المحددة في نهاية قائمة العقد الفرعية للعقدة الحالية (موروث من [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | إدراج عقدة من النوع المحدد في نهاية قائمة العقد الفرعية للعقدة الحالية. (موروث من [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/subsupequationnode/equals/)(object) | تحديد ما إذا كانت عقدة المعادلة الحالية مساوية للعقدة المحددة |
| [GetChild](../../aspose.cells.drawing.equations/equationnode/getchild/)(int) | إرجاع العقدة عند الفهرس المحدد بين أبناء العقدة الحالية. (موروث من [`EquationNode`](../equationnode/).) |
| [InsertAfter](../../aspose.cells.drawing.equations/equationnode/insertafter/)(EquationNodeType) | إدراج العقدة المحددة بعد العقدة الحالية. (موروث من [`EquationNode`](../equationnode/).) |
| [InsertBefore](../../aspose.cells.drawing.equations/equationnode/insertbefore/)(EquationNodeType) | إدراج العقدة المحددة قبل العقدة الحالية. (موروث من [`EquationNode`](../equationnode/).) |
| [InsertChild](../../aspose.cells.drawing.equations/equationnode/insertchild/)(int, EquationNodeType) | إدراج عقدة من النوع المحدد في الموضع الفهرسي المحدد في قائمة العقد الفرعية للعقدة الحالية. (موروث من [`EquationNode`](../equationnode/).) |
| [Remove](../../aspose.cells.drawing.equations/equationnode/remove/)() | إزالة نفسها من الأصل. (موروث من [`EquationNode`](../equationnode/).) |
| [RemoveAllChildren](../../aspose.cells.drawing.equations/equationnode/removeallchildren/)() | إزالة جميع العقد الفرعية للعقدة الحالية. (موروث من [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(EquationNode) | إزالة العقدة المحددة من أبناء العقدة الحالية. (موروث من [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(int) | إزالة العقدة عند الفهرس المحدد من أبناء العقدة الحالية. (موروث من [`EquationNode`](../equationnode/).) |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | تعيين نمط WordArt المسبق. (موروث من [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ToLaTeX](../../aspose.cells.drawing.equations/equationnode/tolatex/)() | تحويل هذه المعادلة إلى تعبير LaTeX. (موروث من [`EquationNode`](../equationnode/).) |
| [ToMathML](../../aspose.cells.drawing.equations/equationnode/tomathml/)() | تحويل هذه المعادلة إلى تعبير MathML. (موروث من [`EquationNode`](../equationnode/).) |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassSubSupEquationNodeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Aspose.Cells.Drawing.TextBox textBox = worksheet.Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            string[] vals = new string[] { "A", "B", "C" };

            // إنشاء معادلة فرعية (A مع الحرف السفلي B)
            SubSupEquationNode subNode = (SubSupEquationNode)mathNode.AddChild(EquationNodeType.Sub);
            AddBaseComponent(subNode, vals[0]);
            AddSubscriptComponent(subNode, vals[1]);

            // إنشاء معادلة علوية (A مع الحرف العلوي C)
            SubSupEquationNode supNode = (SubSupEquationNode)mathNode.AddChild(EquationNodeType.Sup);
            AddBaseComponent(supNode, vals[0]);
            AddSuperscriptComponent(supNode, vals[2]);

            // إنشاء معادلة فرعية وعليا (A مع الحرف السفلي B والحرف العلوي C)
            SubSupEquationNode subSupNode = (SubSupEquationNode)mathNode.AddChild(EquationNodeType.SubSup);
            AddBaseComponent(subSupNode, vals[0]);
            AddSubscriptComponent(subSupNode, vals[1]);
            AddSuperscriptComponent(subSupNode, vals[2]);

            // إنشاء معادلة PreSubSup (الحرف السفلي B، الحرف العلوي C، ثم القاعدة A)
            SubSupEquationNode preSubSupNode = (SubSupEquationNode)mathNode.AddChild(EquationNodeType.PreSubSup);
            AddSubscriptComponent(preSubSupNode, vals[1]);
            AddSuperscriptComponent(preSubSupNode, vals[2]);
            AddBaseComponent(preSubSupNode, vals[0]);

            workbook.Save("SubSupEquationDemo.xlsx");
        }

        private static void AddBaseComponent(SubSupEquationNode parent, string text)
        {
            EquationNode baseNode = parent.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = text;
        }

        private static void AddSubscriptComponent(SubSupEquationNode parent, string text)
        {
            EquationNode subNode = parent.AddChild(EquationNodeType.Subscript);
            TextRunEquationNode textNode = (TextRunEquationNode)subNode.AddChild(EquationNodeType.Text);
            textNode.Text = text;
        }

        private static void AddSuperscriptComponent(SubSupEquationNode parent, string text)
        {
            EquationNode supNode = parent.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode textNode = (TextRunEquationNode)supNode.AddChild(EquationNodeType.Text);
            textNode.Text = text;
        }
    }
}
```

### انظر أيضًا

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


