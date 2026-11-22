---
title: "التعداد ControlMousePointerType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Drawing.ActiveXControls.ControlMousePointerType. يمثل نوع الأيقونة المعروضة كمؤشر الفأرة للتحكم"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/controlmousepointertype/
---
## ControlMousePointerType enumeration

يمثل نوع الأيقونة المعروضة كمؤشر الفأرة للتحكم.

```csharp
public enum ControlMousePointerType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Default | `0` | المؤشر القياسي. |
| Arrow | `1` | سهم. |
| Cross | `2` | مؤشر تقاطع. |
| IBeam | `3` | مؤشر شكل I. |
| SizeNESW | `6` | سهم مزدوج يشير إلى الشمال الشرقي والجنوب الغربي. |
| SizeNS | `7` | سهم مزدوج يشير إلى الشمال والجنوب. |
| SizeNWSE | `8` | سهم مزدوج يشير إلى الشمال الغربي والجنوب الشرقي. |
| SizeWE | `9` | سهم مزدوج يشير إلى الغرب والشرق. |
| UpArrow | `10` | سهم لأعلى. |
| HourGlass | `11` | ساعة رملية. |
| NoDrop | `12` | رمز "ليس" (دائرة بخط مائل) فوق الكائن الجاري سحبه. |
| AppStarting | `13` | سهم مع ساعة رملية. |
| Help | `14` | سهم مع علامة سؤال. |
| SizeAll | `15` | مؤشر "حجم-الكل" (أسهم تشير إلى الشمال والجنوب والشرق والغرب). |
| Custom | `99` | يستخدم الأيقونة المحددة بواسطة خاصية MouseIcon. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlMousePointerTypeDemo
    {
        public static void ControlMousePointerTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة عنصر تحكم ActiveX إلى ورقة العمل
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl control = (ComboBoxActiveXControl)shape.ActiveXControl;

            // حوّل الـActiveXControl إلى ActiveXControlBase للوصول إلى خصائصه
            ActiveXControlBase controlBase = control as ActiveXControlBase;

            if (controlBase != null)
            {
                // حدد نوع مؤشر الفأرة للعنصر
                controlBase.MousePointer = ControlMousePointerType.Cross;

                // حدد خصائص أخرى للعرض
                controlBase.Width = 150;
                controlBase.Height = 50;
                controlBase.IsVisible = true;
                controlBase.Shadow = true;
                controlBase.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Blue);
                controlBase.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.LightGray);
            }

            // احفظ المصنف
            workbook.Save("ControlMousePointerTypeExample.xlsx");
            workbook.Save("ControlMousePointerTypeExample.pdf");

            // أخرج النتيجة.
            Console.WriteLine("Workbook with ActiveX control and custom mouse pointer type saved as 'ControlMousePointerTypeExample.xlsx'.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


