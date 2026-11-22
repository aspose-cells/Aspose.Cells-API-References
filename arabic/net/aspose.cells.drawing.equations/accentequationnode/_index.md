---
title: "الفئة AccentEquationNode"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.Equations.AccentEquationNode. تحدد هذه الفئة معادلة لهجة تتكون من مكوّن أساسي وعلامة تشكيلية مركبة"
type: docs
url: /ar/net/aspose.cells.drawing.equations/accentequationnode/
---
## AccentEquationNode class

تحدد هذه الفئة معادلة لهجة، تتكون من مكون أساسي ومركب تشكيل.

```csharp
public class AccentEquationNode : EquationNode
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AccentCharacter](../../aspose.cells.drawing.equations/accentequationnode/accentcharacter/) { get; set; } | تحدد هذه الخاصية نوع علامة التشكيل المركبة المرفقة بقاعدة دالة اللهجة. الحرف الافتراضي لللهجة هو U+0302. يُنصح بشدة باستخدام الخاصية AccentType لتعيين حرف اللهجة. استخدم إعداد هذه الخاصية إذا لم تتمكن من العثور على الحرف الذي تحتاجه في نوع معروف. |
| [AccentCharacterType](../../aspose.cells.drawing.equations/accentequationnode/accentcharactertype/) { get; set; } | تحديد الأحرف المركبة بقيمة النوع. |
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
| override [Equals](../../aspose.cells.drawing.equations/accentequationnode/equals/)(object) | تحديد ما إذا كانت عقدة المعادلة الحالية مساوية للعقدة المحددة |
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
    public class EquationsClassAccentEquationNodeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة شكل معادلة إلى ورقة العمل الأولى
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // الحصول على عقدة المعادلة
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // إضافة عقدة لهجة
            AccentEquationNode accentNode = (AccentEquationNode)mathNode.AddChild(EquationNodeType.Accent);
            accentNode.AccentCharacter = "\u0302"; // Circumflex accent

            // إضافة عقدة أساسية ونص
            EquationNode baseNode = accentNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "x";

            // احفظ المصنف
            workbook.Save("AccentEquationDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


