---
title: "تعداد EquationMathematicalOperatorType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Drawing.Equations.EquationMathematicalOperatorType enum. نوع عوامل رياضية"
type: docs
url: /ar/net/aspose.cells.drawing.equations/equationmathematicaloperatortype/
---
## EquationMathematicalOperatorType enumeration

نوع عوامل رياضية

```csharp
public enum EquationMathematicalOperatorType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Unknown | `-1` | استخدم النوع غير المعروف عندما لا يتم العثور عليه في النوع الموجود |
| ForAll | `0` | "∀" Unicode:\u2200 |
| Complement | `1` | "∁" Unicode:\u2201 |
| PartialDifferential | `2` | "∂" Unicode:\u2202 |
| Exists | `3` | "∃" Unicode:\u2203 |
| NotExists | `4` | "∄" Unicode:\u2204 |
| EmptySet | `5` | "∅" Unicode:\u2205 |
| Increment | `6` | "∆" Unicode:\u2206 |
| Nabla | `7` | "∇" Unicode:\u2207 |
| ElementOf | `8` | "∈" Unicode:\u2208 |
| NotAnElementOf | `9` | "∉" Unicode:\u2209 |
| SmallElementOf | `10` | "∊" يونيكود:\u220a |
| Contain | `11` | "∋" يونيكود:\u220b |
| NotContain | `12` | "∌" يونيكود:\u220c |
| SmallContain | `13` | "∍" يونيكود:\u220d |
| EndOfProof | `14` | "∎" يونيكود:\u220e |
| NaryProduct | `15` | "∏" يونيكود:\u220f |
| NaryCoproduct | `16` | "∐" يونيكود:\u2210 |
| NarySummation | `17` | "∑" يونيكود:\u2211 |
| LogicalAnd | `18` | "∧" يونيكود:\u2227 |
| LogicalOr | `19` | "∨" يونيكود:\u2228 |
| Intersection | `20` | "∩" يونيكود:\u2229 |
| Union | `21` | "∪" يونيكود:\u222a |
| Integral | `22` | "∫" يونيكود:\u222b |
| DoubleIntegral | `23` | "∬" يونيكود:\u222c |
| TripleIntegral | `24` | "∭" يونيكود:\u222d |
| ContourIntegral | `25` | "∮" يونيكود:\u222e |
| SurfaceIntegral | `26` | "∯" يونيكود:\u222f |
| VolumeIntegral | `27` | "∰" يونيكود:\u2230 |
| Clockwise | `28` | "∱" يونيكود:\u2231 |
| ClockwiseContourIntegral | `29` | "∲" يونيكود:\u2232 |
| AnticlockwiseContourIntegral | `30` | "∳" يونيكود:\u2233 |
| NaryLogicalAnd | `31` | "⋀" يونيكود:\u22c0 |
| NaryLogicalOr | `32` | "⋁" يونيكود:\u22c1 |
| NaryIntersection | `33` | "⋂" يونيكود:\u22c2 |
| NaryUnion | `34` | "⋃" يونيكود:\u22c3 |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationsClassEquationMathematicalOperatorTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف مربع نص لإدراج عوامل رياضية
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 0, 0);
            textBox.Text = "Mathematical Operators Demo:\n";

            // اعرض قيم مختلفة من EquationMathematicalOperatorType
            textBox.Text += $"ForAll: {(char)0x2200}\n";
            textBox.Text += $"Complement: {(char)0x2201}\n";
            textBox.Text += $"PartialDifferential: {(char)0x2202}\n";
            textBox.Text += $"Exists: {(char)0x2203}\n";
            textBox.Text += $"NarySummation: {(char)0x2211}\n";
            textBox.Text += $"LogicalAnd: {(char)0x2227}\n";
            textBox.Text += $"LogicalOr: {(char)0x2228}\n";
            textBox.Text += $"Integral: {(char)0x222B}\n";
            textBox.Text += $"DoubleIntegral: {(char)0x222C}\n";
            textBox.Text += $"NaryLogicalAnd: {(char)0x22C0}\n";

            // استخدام قيم التعداد مباشرة
            EquationMathematicalOperatorType operatorType = EquationMathematicalOperatorType.NarySummation;
            textBox.Text += $"\nSelected operator via enum: {operatorType} ({(char)0x2211})";

            // حفظ النتيجة
            workbook.Save("EquationMathematicalOperatorTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


