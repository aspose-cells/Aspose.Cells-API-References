---
title: "NaryEquationNode.LimitLocation"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية NaryEquationNode. تحدد هذه السمة موقع الحدود في عوامل nary. يمكن أن تكون الحدود إما مركزة فوق وتحت عامل nary أو موضوعة مباشرةً إلى يمين العامل"
type: docs
url: /ar/net/aspose.cells.drawing.equations/naryequationnode/limitlocation/
---
## NaryEquationNode.LimitLocation property

تحدد هذه الخاصية موقع الحدود في عوامل n-ary. يمكن أن تكون الحدود إما متمركزة فوق وتحت عامل n-ary، أو موضوعة مباشرةً إلى يمين العامل.

```csharp
public EquationLimitLocationType LimitLocation { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class NaryEquationNodePropertyLimitLocationDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء شكل لاحتواء المعادلة
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 200, 50);

            // الوصول إلى المعادلة وإضافة عقدة معامل nary
            var equation = shape.GetEquationParagraph();
            var naryNode = equation.AddChild(EquationNodeType.NaryEquation);

            // تحويل إلى NaryEquationNode للوصول إلى LimitLocation
            var naryEquationNode = (NaryEquationNode)naryNode;

            try
            {
                // عرض LimitLocation الحالي (القيمة الافتراضية)
                Console.WriteLine("Default LimitLocation: " + naryEquationNode.LimitLocation);

                // تعيين LimitLocation إلى SubSup (الحدود على الجانب الأيمن)
                naryEquationNode.LimitLocation = EquationLimitLocationType.SubSup;
                Console.WriteLine("After setting to SubSup: " + naryEquationNode.LimitLocation);

                // العودة إلى UndOvr (حدود مركزة)
                naryEquationNode.LimitLocation = EquationLimitLocationType.UndOvr;
                Console.WriteLine("After setting to UndOvr: " + naryEquationNode.LimitLocation);

                // احفظ المصنف
                workbook.Save("LimitLocationDemo.xlsx");
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

* enum [EquationLimitLocationType](../../equationlimitlocationtype/)
* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


