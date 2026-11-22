---
title: "التعداد EquationNodeType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Drawing.Equations.EquationNodeType. نوع عقدة المعادلة. ملاحظة 1199 حاليًا هناك عقدة واحدة فقط في النطاق وقيمة تعدادها هي 1. العقدة التي يحددها تُستخدم لتخزين النص الرياضي. 2100199 يشير إلى أن العقدة مكوّن لبعض عقد الدوال الخاصة. 3200 يشير إلى أن العقدة لديها بعض الدوال الخاصة"
type: docs
url: /ar/net/aspose.cells.drawing.equations/equationnodetype/
---
## EquationNodeType enumeration

نوع عقدة المعادلة. ملاحظة: (1)[1-99] حالياً هناك عقدة واحدة فقط في النطاق، وقيمة تعدادها هي 1. العقدة التي يحددها تُستخدم لتخزين النص الرياضي. (2)[100-199] تشير إلى أن العقدة مكوّن لبعض عقد الدوال الخاصة. (3)[200-] تشير إلى أن للعقدة بعض الدوال الخاصة.

```csharp
public enum EquationNodeType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| UnKnow | `0` | UnKnow |
| Text | `1` | يحدد عقدة تخزن نصًا رياضيًا |
| Base | `100` | يحدد مكوّن Base |
| Denominator | `101` | يحدد مكوّن Denominator |
| Numerator | `102` | يحدد مكوّن Numerator |
| FunctionName | `103` | يحدد مكوّن FunctionName |
| Subscript | `104` | يحدد مكوّن Subscript |
| Superscript | `105` | يحدد مكوّن Superscript |
| Degree | `106` | يحدد مكوّن Degree |
| MatrixRow | `107` | يحدد مكوّن MatrixRow. صف واحد من المصفوفة |
| Limit | `108` | يمثل كائنًا فرعيًا لدالة Lower-Limit أو دالة Upper-Limit |
| EquationParagraph | `200` | يحدد فقرة رياضية(oMathPara). |
| MathematicalEquation | `201` | يحدد معادلة أو تعبير رياضي(OMath). |
| FractionEquation | `202` | يحدد معادلة كسرية |
| FunctionEquation | `203` | يحدد معادلة دالة |
| DelimiterEquation | `204` | يحدد معادلة محدد |
| NaryEquation | `205` | يحدد معادلة عامل n-ary |
| RadicalEquation | `206` | يحدد المعادلة الجذرية |
| SuperscriptEquation | `207` | يحدد معادلة أُس |
| SubscriptEquation | `208` | يحدد معادلة أس سفلي |
| SubSupEquation | `209` | يحدد معادلة ذات أسس وأس سفلي إلى يمين المتعاملات. |
| PreSubSupEquation | `210` | يحدد معادلة ذات أسس وأس سفلي إلى يسار المتعاملات. |
| AccentEquation | `211` | يحدد معادلة إشارة |
| BarEquation | `212` | يحدد معادلة شريط |
| BorderBoxEquation | `213` | يحدد معادلة صندوق حدودي |
| BoxEquation | `214` | يحدد معادلة صندوق |
| GroupCharacterEquation | `215` | يحدد معادلة مجموعة-حرف |
| MatrixEquation | `216` | يحدد معادلة المصفوفة، |
| LowerLimit | `217` | يحدد دالة الحد الأدنى |
| UpperLimit | `218` | يحدد دالة الحد الأعلى |
| Mathematical | `201` | يحدد معادلة أو تعبير رياضي(OMath). |
| Fraction | `202` | يحدد معادلة كسرية |
| Function | `203` | يحدد معادلة دالة |
| Delimiter | `204` | يحدد معادلة محدد |
| Nary | `205` | يحدد معادلة عامل n-ary |
| Radical | `206` | يحدد المعادلة الجذرية |
| Sup | `207` | يحدد معادلة أُس |
| Sub | `208` | يحدد معادلة أس سفلي |
| SubSup | `209` | يحدد معادلة ذات أسس وأس سفلي إلى يمين المتعاملات. |
| PreSubSup | `210` | يحدد معادلة ذات أسس وأس سفلي إلى يسار المتعاملات. |
| Accent | `211` | يحدد معادلة إشارة |
| Bar | `212` | يحدد معادلة شريط |
| BorderBox | `213` | يحدد معادلة صندوق حدودي |
| Box | `214` | يحدد معادلة صندوق |
| GroupChr | `215` | يحدد معادلة مجموعة-حرف |
| Matrix | `216` | يحدد معادلة المصفوفة، |
| ArrayEquation | `317` | يحدد دالة مصفوفة المعادلات. تتكون الدالة من معادلة واحدة أو أكثر. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationNodeTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة معادلة إلى ورقة العمل الأولى
            var equationShape = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // احصل على عقدة الرياضيات من المعادلة
            EquationNode mathNode = equationShape.GetEquationParagraph().GetChild(0);

            // أنشئ عقدة إشارة مع حرف circumflex
            AccentEquationNode accentNode = (AccentEquationNode)mathNode.AddChild(EquationNodeType.Accent);
            accentNode.AccentCharacter = "\u0302";

            // أضف عقدة الأساس وعقدة النص
            EquationNode baseNode = accentNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "x";

            // احفظ المصنف
            workbook.Save("EquationNodeTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


