---
title: "ShapeCollection.AddLaTeXEquation"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. يضيف كائن معادلة إلى ورقة العمل باستخدام سلاسل تنسيق LaTeX"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addlatexequation/
---
## ShapeCollection.AddLaTeXEquation method

يضيف كائن معادلة إلى ورقة العمل باستخدام سلاسل تنسيق LaTeX.

```csharp
public TextBox AddLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, 
    int width, string latex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | Int32 | فهرس الصف العلوي. |
| أعلى | Int32 | الإزاحة العمودية للصف العلوي، بوحدة البكسل. |
| العمود الأيسر | Int32 | فهرس العمود الأيسر. |
| يسار | Int32 | الإزاحة الأفقية من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | Int32 | ارتفاع المعادلة، بوحدة البكسل. |
| العرض | Int32 | عرض المعادلة، بوحدة البكسل. |
| لاتكس | String | سلسلة تنسيق LaTeX |

### أمثلة

```csharp

[C#]
// سلسلة تنسيق LaTeX.
string latex = "\\alpha +  \\frac{\\partial^2}{\\partial x_1\\partial x_2}y - \\left ( a + b \\right )+_{a}^{b}\\beta";
// يضيف كائن معادلة إلى ورقة العمل.
TextBox textBox = shapes.AddLaTeXEquation(1, 0, 1, 0, 100, 300, latex);
```

### انظر أيضًا

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


