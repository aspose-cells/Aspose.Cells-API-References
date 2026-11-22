---
title: "التعداد EquationLimitLocationType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Drawing.Equations.EquationLimitLocationType. يحدد موقع الحد على العامل"
type: docs
url: /ar/net/aspose.cells.drawing.equations/equationlimitlocationtype/
---
## EquationLimitLocationType enumeration

يحدد موقع الحد على العامل.

```csharp
public enum EquationLimitLocationType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| UndOvr | `0` | يحدد أن الحد يكون مركّزًا فوق أو تحت العامل. |
| SubSup | `1` | يحدد أن الحد يكون على الجانب الأيمن من العامل. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationsClassEquationLimitLocationTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // أضف شكل معادلة إلى ورقة العمل
                TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

                // احصل على فقرة المعادلة والطفل الأول لها
                EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

                // أنشئ عقدة معادلة Nary
                NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);

                // عيّن موقع الحد إلى SubSup (الجانب الأيمن من العامل)
                naryNode.LimitLocation = EquationLimitLocationType.SubSup;
                Console.WriteLine("Limit location set to SubSup: " + naryNode.LimitLocation);

                // أضف بعض المحتوى إلى المعادلة
                EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
                TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
                textNode.Text = "x";

                // غيّر إلى UndOvr (مركّز فوق/تحت العامل)
                naryNode.LimitLocation = EquationLimitLocationType.UndOvr;
                Console.WriteLine("Limit location changed to UndOvr: " + naryNode.LimitLocation);

                // احفظ المصنف
                workbook.Save("EquationLimitLocationTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


