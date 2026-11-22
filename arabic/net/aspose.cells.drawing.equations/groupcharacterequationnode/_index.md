---
title: "الفئة GroupCharacterEquationNode"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.Equations.GroupCharacterEquationNode. تحدد هذه الفئة وظيفة GroupCharacter التي تتكون من حرف يُرسم فوق أو تحت النص غالبًا بهدف تجميع العناصر بصريًا"
type: docs
url: /ar/net/aspose.cells.drawing.equations/groupcharacterequationnode/
---
## GroupCharacterEquationNode class

هذه الفئة تحدد دالة Group-Character، التي تتكون من حرف يُرسم فوق أو تحت النص، غالبًا بهدف تجميع العناصر بصريًا.

```csharp
public class GroupCharacterEquationNode : EquationNode
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ChrType](../../aspose.cells.drawing.equations/groupcharacterequationnode/chrtype/) { get; set; } | تحديد الأحرف المركبة بقيمة النوع. |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | احصل على نوع المعادلة للعقدة الحالية (موروث من [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | يعيد الخط لهذا الكائن. (موروث من [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [GroupChr](../../aspose.cells.drawing.equations/groupcharacterequationnode/groupchr/) { get; set; } | يحدد رمزًا (الافتراضي U+23DF). يُنصح بشدة باستخدام السمة ChrType لتعيين حرف التشكيل. استخدم إعداد الخاصية هذا إذا لم تتمكن من العثور على الحرف الذي تحتاجه في نوع معروف. |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | يحصل على طول الأحرف. (موروث من [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | يحدد العقدة الأب للعقدة الحالية (موروث من [`EquationNode`](../equationnode/).) |
| [Position](../../aspose.cells.drawing.equations/groupcharacterequationnode/position/) { get; set; } | هذه السمة تحدد موضع الحرف في الكائن |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | يحصل على الفهرس الابتدائي للأحرف. (موروث من [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | يعيد خيارات النص. (موروث من [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | يمثل نوع العقدة (موروث من [`EquationNode`](../equationnode/).) |
| [VertJc](../../aspose.cells.drawing.equations/groupcharacterequationnode/vertjc/) { get; set; } | هذه السمة، مع الجمع مع pos في groupChrPr، تحدد التخطيط العمودي لكائن groupChr. حيث يحدد pos موضع حرف التجميع، ويحدد vertJc محاذاة الكائن بالنسبة للخط الأساسي. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | يدرج العقدة المحددة في نهاية قائمة العقد الفرعية للعقدة الحالية (موروث من [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | إدراج عقدة من النوع المحدد في نهاية قائمة العقد الفرعية للعقدة الحالية. (موروث من [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/groupcharacterequationnode/equals/)(object) | تحديد ما إذا كانت عقدة المعادلة الحالية مساوية للعقدة المحددة |
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
    public class EquationsClassGroupCharacterEquationNodeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة شكل معادلة
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            // احصل على عقدة الرياضيات وأضف حرف التجميع
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            GroupCharacterEquationNode groupCharNode = (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
            
            // تكوين خصائص حرف التجميع
            groupCharNode.Position = EquationCharacterPositionType.Top;
            groupCharNode.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;
            
            // أضف النص الأساسي
            EquationNode baseNode = groupCharNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "abc";
            
            // احفظ المصنف
            workbook.Save("GroupCharacterEquationDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


