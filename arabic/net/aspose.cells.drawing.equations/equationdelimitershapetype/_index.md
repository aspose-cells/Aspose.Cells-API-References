---
title: "التعداد EquationDelimiterShapeType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Drawing.Equations.EquationDelimiterShapeType. يحدد هذا شكل الفواصل في كائن الفاصل"
type: docs
url: /ar/net/aspose.cells.drawing.equations/equationdelimitershapetype/
---
## EquationDelimiterShapeType enumeration

هذا يحدد شكل الفواصل في كائن الفاصل.

```csharp
public enum EquationDelimiterShapeType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Centered | `0` | المقسم يتمركز حول الارتفاع الكامل لمحتواه. |
| Match | `1` | المقسم يتم تعديلها لتطابق تمامًا ارتفاع محتواها. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationDelimiterShapeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة شكل معادلة
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            // الحصول على عقدة المعادلة
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // إنشاء عقدة فاصل بنوع الشكل Match
            DelimiterEquationNode delimiterNode = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
            delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;
            delimiterNode.BeginChar = "{";
            delimiterNode.EndChar = "}";
            
            // إضافة محتوى داخل الفاصل
            EquationNode baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "Content";
            
            // احفظ المصنف
            workbook.Save("EquationDelimiterShapeTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


