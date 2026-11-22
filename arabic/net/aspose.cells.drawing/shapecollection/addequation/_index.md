---
title: "ShapeCollection.AddEquation"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. تضيف كائن معادلة إلى ورقة العمل"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addequation/
---
## ShapeCollection.AddEquation method

يضيف كائن معادلة إلى ورقة العمل.

```csharp
public TextBox AddEquation(int topRow, int top, int leftColumn, int left, int height, int width)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | Int32 | فهرس الصف العلوي. |
| أعلى | Int32 | الإزاحة العمودية للصف العلوي، بوحدة البكسل. |
| العمود الأيسر | Int32 | فهرس العمود الأيسر. |
| يسار | Int32 | الإزاحة الأفقية من عموده الأيسر، بوحدة البكسل. |
| الارتفاع | Int32 | ارتفاع المعادلة، بوحدة البكسل. |
| العرض | Int32 | عرض المعادلة، بوحدة البكسل. |

### أمثلة

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddEquationWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            FractionEquationNode fraction = (FractionEquationNode)mathNode.AddChild(EquationNodeType.Fraction);
            fraction.FractionType = EquationFractionType.Skewed;

            EquationComponentNode numerator = (EquationComponentNode)fraction.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode numText = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            numText.Text = "A";

            EquationComponentNode denominator = (EquationComponentNode)fraction.AddChild(EquationNodeType.Denominator);
            TextRunEquationNode denText = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            denText.Text = "B";

            workbook.Save("ShapeEquationDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


