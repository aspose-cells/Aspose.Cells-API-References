---
title: "التعداد EquationCombiningCharacterType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Drawing.Equations.EquationCombiningCharacterType. نوع الأحرف المدمجة"
type: docs
url: /ar/net/aspose.cells.drawing.equations/equationcombiningcharactertype/
---
## EquationCombiningCharacterType enumeration

نوع الأحرف المدمجة.

```csharp
public enum EquationCombiningCharacterType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Unknown | `-1` | استخدم النوع غير المعروف عندما لا يتم العثور عليه في النوع الموجود |
| DotAbove | `0` | "̇" Unicode: u0307 نقطة مركبة فوق |
| Diaeresis | `1` | "̈" Unicode: u0308 نقطتان مركبتان فوق |
| ThreeDotsAbove | `2` | "⃛" Unicode: u20db ثلاث نقاط مركبة فوق |
| CircumflexAccent | `3` | "̂" Unicode: u0302 اللكنة المرفوعة المركبة |
| Caron | `4` | "̌" Unicode: u030c الكارون المركب |
| AcuteAccent | `5` | "́" Unicode: u0301 اللكنة الحادة المركبة |
| GraveAccent | `6` | "̀" Unicode: u0300 اللكنة المكسورة المركبة |
| Breve | `7` | "̆" Unicode: u0306 دمج البريف |
| Tilde | `8` | "̃" Unicode: u0303 التيليدة المركبة |
| Overline | `9` | "̅" Unicode: u0305 الخط العلوي المركب |
| DoubleOverline | `10` | "̿" Unicode: u033f الخط العلوي المزدوج المركب |
| TopCurlyBracket | `11` | "⏞" Unicode: u23de القوس المعقوف العلوي المركب |
| BottomCurlyBracket | `12` | "⏟" Unicode: u23df الجمع بين القوس المتعرج السفلي |
| LeftArrowAbove | `13` | "⃖" Unicode: u20d6 الجمع بين السهم الأيسر أعلاه |
| RightArrowAbove | `14` | "⃗" Unicode: u20d7 الجمع بين السهم الأيمن أعلاه |
| LeftRightArrowAbove | `15` | "⃡" Unicode: u20e1 الجمع بين السهمين الأيسر والأيمن أعلاه |
| LeftHarpoonAbove | `16` | "⃐" Unicode: u20d0 الجمع بين الخطاف الأيسر أعلاه |
| RightHarpoonAbove | `17` | "⃑" Unicode: u20d1 الجمع بين الخطاف الأيمن أعلاه |
| LeftwardsArrow | `18` | "←" Unicode: u2190 السهم المتجه إلى اليسار |
| RightwardsArrow | `19` | "→" Unicode: u2192 السهم المتجه إلى اليمين |
| LeftRightArrow | `20` | "↔" Unicode: u2194 السهم المتجه يمينًا ويسارًا |
| LeftwardsDoubleArrow | `21` | "⇐" Unicode: u21d0 السهم المزدوج المتجه إلى اليسار |
| RightwardsDoubleArrow | `22` | "⇒" Unicode: u21d2 السهم المزدوج المتجه إلى اليمين |
| LeftRightDoubleArrow | `23` | "⇔" Unicode: u21d4 السهم المزدوج المتجه يمينًا ويسارًا |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationCombiningCharacterTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            GroupCharacterEquationNode node = (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
            node.Position = EquationCharacterPositionType.Top;
            node.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;

            EquationNode subBase = node.AddChild(EquationNodeType.Base);
            TextRunEquationNode textRun = (TextRunEquationNode)(subBase.AddChild(EquationNodeType.Text));
            textRun.Text = "abc";

            string resultFile = "GroupCharacterEquationTest.xlsx";
            workbook.Save(resultFile);

            // تحقق من الملف المحفوظ
            Workbook workbook2 = new Workbook(resultFile);
            TextBox textBoxRead = (TextBox)workbook2.Worksheets[0].Shapes[0];
            EquationNode mathNode2 = textBoxRead.GetEquationParagraph().GetChild(0);
            GroupCharacterEquationNode node2 = (GroupCharacterEquationNode)mathNode2.GetChild(0);

            Console.WriteLine("Equation Type: " + node2.EquationType);
            Console.WriteLine("Position: " + node2.Position);
            Console.WriteLine("Character Type: " + node2.ChrType);
            Console.WriteLine("Group Character: " + node2.GroupChr);

            EquationNode baseNode = node2.GetChild(0);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.GetChild(0);
            Console.WriteLine("Text Content: " + textNode.Text);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


