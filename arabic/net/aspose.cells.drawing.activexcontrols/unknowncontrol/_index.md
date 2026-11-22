---
title: "الفئة UnknownControl"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.ActiveXControls.UnknownControl. عنصر تحكم غير معروف"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/unknowncontrol/
---
## UnknownControl class

تحكم غير معروف.

```csharp
public class UnknownControl : ActiveXControl
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | يحصل ويضبط لون الـole للخلفية. (موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| override [Data](../../aspose.cells.drawing.activexcontrols/unknowncontrol/data/) { get; } | يحصل على البيانات الثنائية للعنصر ويضبطها. |
| [Font](../../aspose.cells.drawing.activexcontrols/activexcontrol/font/) { get; } | يمثّل خط العنصر. (موروث من [`ActiveXControl`](../activexcontrol/).) |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/) { get; set; } | يحصل ويضبط لون الـole للمقدمة. (موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height/) { get; set; } | يحصل ويضبط ارتفاع العنصر بوحدة النقاط. (موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [IMEMode](../../aspose.cells.drawing.activexcontrols/activexcontrol/imemode/) { get; set; } | يحصل ويضبط وضع التشغيل الافتراضي لمحرّر طريقة الإدخال للعنصر عند حصوله على التركيز. (موروث من [`ActiveXControl`](../activexcontrol/).) |
| virtual [IsAutoSize](../../aspose.cells.drawing.activexcontrols/activexcontrol/isautosize/) { get; set; } | يشير إلى ما إذا كان العنصر سيعيد حجمه تلقائيًا لعرض محتوياته بالكامل. (موروث من [`ActiveXControl`](../activexcontrol/).) |
| [IsEnabled](../../aspose.cells.drawing.activexcontrols/activexcontrol/isenabled/) { get; set; } | يشير إلى ما إذا كان العنصر يمكنه استلام التركيز والاستجابة للأحداث التي يولدها المستخدم. (موروث من [`ActiveXControl`](../activexcontrol/).) |
| [IsLocked](../../aspose.cells.drawing.activexcontrols/activexcontrol/islocked/) { get; set; } | يشير إلى ما إذا كانت البيانات في العنصر مقفلة للتحرير. (موروث من [`ActiveXControl`](../activexcontrol/).) |
| [IsTransparent](../../aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/) { get; set; } | يشير إلى ما إذا كان التحكم شفافًا.(موروث من [`ActiveXControl`](../activexcontrol/).) |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/) { get; set; } | يشير إلى ما إذا كان هذا التحكم مرئيًا.(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | يحصل على الخلية المرتبطة ويضبطها.(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | يحصل على نطاق تعبئة القائمة ويضبطه.(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | يحصل على أيقونة مخصصة لعرضها كمؤشر الفأرة للتحكم ويضبطها.(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | يحصل على نوع الأيقونة المعروضة كمؤشر الفأرة للتحكم ويضبطه.(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | يشير إلى ما إذا كان يجب إظهار ظل.(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | يمثل طريقة محاذاة النص المستخدم في التحكم.(موروث من [`ActiveXControl`](../activexcontrol/).) |
| override [Type](../../aspose.cells.drawing.activexcontrols/unknowncontrol/type/) { get; } | يحصل على نوع عنصر التحكم ActiveX. |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | يحصل على عرض التحكم بوحدة النقاط ويضبطه.(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | يحصل على كائن [`Workbook`](../activexcontrolbase/workbook/).(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetRelationshipData](../../aspose.cells.drawing.activexcontrols/unknowncontrol/getrelationshipdata/)(string) | يحصل على البيانات المرتبطة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ActiveXControlsClassUnknownControlDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر تحكم Unknown ActiveX إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.Unknown,
                0,  // topRow
                0,  // top
                0,  // leftColumn
                0,  // left
                100,// width
                50  // height
            );

            // احصل على نسخة UnknownControl من الشكل
            UnknownControl unknownControl = (UnknownControl)shape.ActiveXControl;
            unknownControl.IsVisible = true;

            // احفظ المصنف
            workbook.Save("UnknownControlDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ActiveXControl](../activexcontrol/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


