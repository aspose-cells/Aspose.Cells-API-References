---
title: "فئة NaryEquationNode"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Drawing.Equations.NaryEquationNode فئة. تحدد هذه الفئة معادلة عامل nary تتكون من عامل nary أساسي أو معامل وحدود علوية وسفلية اختيارية"
type: docs
url: /ar/net/aspose.cells.drawing.equations/naryequationnode/
---
## NaryEquationNode class

هذه الفئة تحدد معادلة عامل n-ary تتكون من عامل n-ary، قاعدة (أو مُعامل)، وحدود علوية وسفلية اختيارية.

```csharp
public class NaryEquationNode : EquationNode
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | احصل على نوع المعادلة للعقدة الحالية (موروث من [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | يعيد الخط لهذا الكائن. (موروث من [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [IsHideSubscript](../../aspose.cells.drawing.equations/naryequationnode/ishidesubscript/) { get; set; } | ما إذا كان سيتم عرض الحد السفلي |
| [IsHideSuperscript](../../aspose.cells.drawing.equations/naryequationnode/ishidesuperscript/) { get; set; } | ما إذا كان سيتم عرض الحد العلوي |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | يحصل على طول الأحرف. (موروث من [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [LimitLocation](../../aspose.cells.drawing.equations/naryequationnode/limitlocation/) { get; set; } | تحدد هذه الخاصية موقع الحدود في عوامل n-ary. يمكن أن تكون الحدود إما متمركزة فوق وتحت عامل n-ary، أو موضوعة مباشرةً إلى يمين العامل. |
| [NaryGrow](../../aspose.cells.drawing.equations/naryequationnode/narygrow/) { get; set; } | تحدد هذه الخاصية خاصية النمو لعوامل n-ary على مستوى المستند. عندما تكون معطلة، لا تنمو عوامل n-ary مثل التكاملات والمجاميع لتطابق حجم ارتفاع المعامل الخاص بها. عندما تكون مفعلة، ينمو عامل n-ary عموديًا ليتطابق مع ارتفاع معاملاته. |
| [NaryOperator](../../aspose.cells.drawing.equations/naryequationnode/naryoperator/) { get; set; } | عامل n-ary. على سبيل المثال "∑". يُنصح بشدة باستخدام الخاصية NaryOperatorType لتعيين عامل n-ary. استخدم هذا الإعداد إذا لم تتمكن من العثور على الحرف الذي تحتاجه في نوع معروف. |
| [NaryOperatorType](../../aspose.cells.drawing.equations/naryequationnode/naryoperatortype/) { get; set; } | عامل n-ary. على سبيل المثال "∑" |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | يحدد العقدة الأب للعقدة الحالية (موروث من [`EquationNode`](../equationnode/).) |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | يحصل على الفهرس الابتدائي للأحرف. (موروث من [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | يعيد خيارات النص. (موروث من [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | يمثل نوع العقدة (موروث من [`EquationNode`](../equationnode/).) |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | يدرج العقدة المحددة في نهاية قائمة العقد الفرعية للعقدة الحالية (موروث من [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | إدراج عقدة من النوع المحدد في نهاية قائمة العقد الفرعية للعقدة الحالية. (موروث من [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/naryequationnode/equals/)(object) | تحديد ما إذا كانت عقدة المعادلة الحالية مساوية للعقدة المحددة |
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
    public class EquationsClassNaryEquationNodeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكل معادلة
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // الحصول على عقدة المعادلة
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // أنشئ عقدة معادلة nary
            NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            
            // عيّن خصائص nary
            naryNode.NaryOperator = "∫";
            naryNode.IsHideSubscript = true;
            naryNode.IsHideSuperscript = true;
            naryNode.NaryGrow = false;

            // أضف المكوّن الأساسي
            EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x";

            // احفظ المصنف
            workbook.Save("NaryEquationDemo.xlsx");

            Console.WriteLine("Nary equation demo created successfully.");
        }
    }
}
```

### انظر أيضًا

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


