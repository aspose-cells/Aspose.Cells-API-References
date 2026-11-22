---
title: "فئة ActiveXControl"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Drawing.ActiveXControls.ActiveXControl. تمثل عنصر التحكم ActiveX"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/activexcontrol/
---
## ActiveXControl class

يمثل عنصر التحكم ActiveX.

```csharp
public abstract class ActiveXControl : ActiveXControlBase
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | يحصل ويضبط لون الـole للخلفية. (موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| override [Data](../../aspose.cells.drawing.activexcontrols/activexcontrol/data/) { get; } | يحصل على البيانات الثنائية للعنصر ويضبطها. |
| [Font](../../aspose.cells.drawing.activexcontrols/activexcontrol/font/) { get; } | يمثل خط العنصر. |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/) { get; set; } | يحصل ويضبط لون الـole للمقدمة. (موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height/) { get; set; } | يحصل ويضبط ارتفاع العنصر بوحدة النقاط. (موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [IMEMode](../../aspose.cells.drawing.activexcontrols/activexcontrol/imemode/) { get; set; } | يحصل على وضع وقت التشغيل الافتراضي لمحرر طريقة الإدخال للعنصر عند استلامه للتركيز ويضبطه. |
| virtual [IsAutoSize](../../aspose.cells.drawing.activexcontrols/activexcontrol/isautosize/) { get; set; } | يشير إلى ما إذا كان العنصر سيعيد حجمه تلقائيًا لعرض محتوياته بالكامل. |
| [IsEnabled](../../aspose.cells.drawing.activexcontrols/activexcontrol/isenabled/) { get; set; } | يشير إلى ما إذا كان العنصر يمكنه استلام التركيز والاستجابة للأحداث التي يولدها المستخدم. |
| [IsLocked](../../aspose.cells.drawing.activexcontrols/activexcontrol/islocked/) { get; set; } | يشير إلى ما إذا كانت البيانات في العنصر مقفلة للتحرير. |
| [IsTransparent](../../aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/) { get; set; } | يشير إلى ما إذا كان العنصر شفافًا. |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/) { get; set; } | يشير إلى ما إذا كان هذا التحكم مرئيًا.(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | يحصل على الخلية المرتبطة ويضبطها.(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | يحصل على نطاق تعبئة القائمة ويضبطه.(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | يحصل على أيقونة مخصصة لعرضها كمؤشر الفأرة للتحكم ويضبطها.(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | يحصل على نوع الأيقونة المعروضة كمؤشر الفأرة للتحكم ويضبطه.(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | يشير إلى ما إذا كان يجب إظهار ظل.(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | يمثل طريقة محاذاة النص المستخدم في العنصر. |
| abstract [Type](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/type/) { get; } | يحصل على نوع عنصر التحكم ActiveX. (موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | يحصل على عرض التحكم بوحدة النقاط ويضبطه.(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | يحصل على كائن [`Workbook`](../activexcontrolbase/workbook/).(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlsClassActiveXControlDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة عنصر تحكم ActiveX من نوع RadioButton
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.RadioButton, 
                1, 1,  // upper left row/column
                1, 1,  // upper left row/column offsets
                100, 30);  // width and height
            RadioButtonActiveXControl radioButton = (RadioButtonActiveXControl)shape.ActiveXControl;

            // تعيين الخصائص
            radioButton.GroupName = "Sheet1";
            radioButton.Alignment = ControlCaptionAlignmentType.Left;
            radioButton.IsWordWrapped = true;
            radioButton.Caption = "OptionButton1";
            radioButton.PicturePosition = ControlPicturePositionType.AboveCenter;
            radioButton.SpecialEffect = ControlSpecialEffectType.Sunken;
            radioButton.IsEnabled = true;
            radioButton.IsTransparent = false;
            radioButton.IsAutoSize = false;
            radioButton.IMEMode = InputMethodEditorMode.NoControl;
            radioButton.Font.Name = "Calibri";
            radioButton.MousePointer = ControlMousePointerType.Default;

            // احفظ المصنف
            workbook.Save("ActiveXControlDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ActiveXControlBase](../activexcontrolbase/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


