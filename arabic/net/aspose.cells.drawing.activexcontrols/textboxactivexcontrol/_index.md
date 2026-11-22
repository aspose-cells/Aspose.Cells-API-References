---
title: "فئة TextBoxActiveXControl"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl. تمثل عنصر تحكم ActiveX TextBox"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/
---
## TextBoxActiveXControl class

يمثل عنصر تحكم ActiveX من نوع text box.

```csharp
public class TextBoxActiveXControl : ActiveXControl
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | يحصل ويضبط لون الـole للخلفية. (موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [BorderOleColor](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/borderolecolor/) { get; set; } | يحصل ويضبط لون الـole للخلفية. |
| [BorderStyle](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/borderstyle/) { get; set; } | يحصل ويضبط نوع الإطار المستخدم من قبل العنصر. |
| override [Data](../../aspose.cells.drawing.activexcontrols/activexcontrol/data/) { get; } | يحصل ويضبط البيانات الثنائية للعنصر. (موروث من [`ActiveXControl`](../activexcontrol/).) |
| [DropButtonStyle](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/dropbuttonstyle/) { get; set; } | يحدد الرمز المعروض على زر السقوط |
| [EnterFieldBehavior](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/enterfieldbehavior/) { get; set; } | يحدد سلوك الاختيار عند دخول العنصر. True يعني أن الاختيار يبقى دون تغيير منذ آخر مرة كان فيها العنصر نشطًا. False يعني أنه سيتم تحديد كل النص داخل العنصر عند الدخول إليه. |
| [EnterKeyBehavior](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/enterkeybehavior/) { get; set; } | يحدد سلوك مفتاح ENTER. true يعني أن ضغط ENTER سيُنشئ سطرًا جديدًا. false يعني أن ضغط ENTER سينقل التركيز إلى العنصر التالي في ترتيب التبويب. |
| [Font](../../aspose.cells.drawing.activexcontrols/activexcontrol/font/) { get; } | يمثّل خط العنصر. (موروث من [`ActiveXControl`](../activexcontrol/).) |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/) { get; set; } | يحصل ويضبط لون الـole للمقدمة. (موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height/) { get; set; } | يحصل ويضبط ارتفاع العنصر بوحدة النقاط. (موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [HideSelection](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/hideselection/) { get; set; } | يشير إلى ما إذا كان النص المحدد في العنصر يظهر مميزًا عندما لا يكون للعنصر تركيز. |
| [IMEMode](../../aspose.cells.drawing.activexcontrols/activexcontrol/imemode/) { get; set; } | يحصل ويضبط وضع التشغيل الافتراضي لمحرّر طريقة الإدخال للعنصر عند حصوله على التركيز. (موروث من [`ActiveXControl`](../activexcontrol/).) |
| [IntegralHeight](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/integralheight/) { get; set; } | يُشير إلى ما إذا كان العنصر سيعرض فقط أسطر النص الكاملة دون إظهار أي أسطر جزئية. |
| virtual [IsAutoSize](../../aspose.cells.drawing.activexcontrols/activexcontrol/isautosize/) { get; set; } | يشير إلى ما إذا كان العنصر سيعيد حجمه تلقائيًا لعرض محتوياته بالكامل. (موروث من [`ActiveXControl`](../activexcontrol/).) |
| [IsAutoTab](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/isautotab/) { get; set; } | يشير إلى ما إذا كان التركيز سيتحرك تلقائيًا إلى العنصر التالي عندما يدخل المستخدم الحد الأقصى لعدد الأحرف. |
| virtual [IsAutoWordSelected](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/isautowordselected/) { get; set; } | يحدد الوحدة الأساسية المستخدمة لتوسيع الاختيار. True يعني أن الوحدة الأساسية هي حرف واحد. false يعني أن الوحدة الأساسية هي كلمة كاملة. |
| [IsDragBehaviorEnabled](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/isdragbehaviorenabled/) { get; set; } | يشير إلى ما إذا كان السحب والإفلات مفعّلاً للعنصر. |
| [IsEditable](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/iseditable/) { get; set; } | يشير إلى ما إذا كان المستخدم يستطيع الكتابة في العنصر. |
| [IsEnabled](../../aspose.cells.drawing.activexcontrols/activexcontrol/isenabled/) { get; set; } | يشير إلى ما إذا كان العنصر يمكنه استلام التركيز والاستجابة للأحداث التي يولدها المستخدم. (موروث من [`ActiveXControl`](../activexcontrol/).) |
| [IsLocked](../../aspose.cells.drawing.activexcontrols/activexcontrol/islocked/) { get; set; } | يشير إلى ما إذا كانت البيانات في العنصر مقفلة للتحرير. (موروث من [`ActiveXControl`](../activexcontrol/).) |
| [IsMultiLine](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/ismultiline/) { get; set; } | يشير إلى ما إذا كان العنصر يمكنه عرض أكثر من سطر واحد من النص. |
| [IsTransparent](../../aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/) { get; set; } | يشير إلى ما إذا كان التحكم شفافًا.(موروث من [`ActiveXControl`](../activexcontrol/).) |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/) { get; set; } | يشير إلى ما إذا كان هذا التحكم مرئيًا.(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [IsWordWrapped](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/iswordwrapped/) { get; set; } | يشير إلى ما إذا كان محتوى العنصر يلتف تلقائيًا في نهاية السطر. |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | يحصل على الخلية المرتبطة ويضبطها.(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | يحصل على نطاق تعبئة القائمة ويضبطه.(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MaxLength](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/maxlength/) { get; set; } | يحصل على الحد الأقصى لعدد الأحرف ويضبطه |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | يحصل على أيقونة مخصصة لعرضها كمؤشر الفأرة للتحكم ويضبطها.(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | يحصل على نوع الأيقونة المعروضة كمؤشر الفأرة للتحكم ويضبطه.(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [PasswordChar](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/passwordchar/) { get; set; } | يحصل ويضبط حرفًا يتم عرضه بدلاً من الأحرف المدخلة. |
| [ScrollBars](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/scrollbars/) { get; set; } | يشير إلى ما إذا كان العنصر يحتوي على أشرطة تمرير عمودية، أشرطة تمرير أفقية، كليهما، أو لا شيء. |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | يشير إلى ما إذا كان يجب إظهار ظل.(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ShowDropButtonTypeWhen](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/showdropbuttontypewhen/) { get; set; } | يحدد الرمز المعروض على زر السقوط |
| [SpecialEffect](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/specialeffect/) { get; set; } | يحصل على التأثير الخاص للتحكم ويضبطه. |
| [TabKeyBehavior](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/tabkeybehavior/) { get; set; } | يشير إلى ما إذا كان مسموحًا بأحرف الجدولة في نص العنصر. |
| [Text](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/text/) { get; set; } | يحصل ويضبط نص العنصر. |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | يمثل طريقة محاذاة النص المستخدم في التحكم.(موروث من [`ActiveXControl`](../activexcontrol/).) |
| override [Type](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/type/) { get; } | يحصل على نوع عنصر التحكم ActiveX. |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | يحصل على عرض التحكم بوحدة النقاط ويضبطه.(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | يحصل على كائن [`Workbook`](../activexcontrolbase/workbook/).(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class TextBoxActiveXControlDemo
    {
        public static void TextBoxActiveXControlExample()
        {
            // تهيئة دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة TextBoxActiveXControl
            Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(ControlType.TextBox, 1, 0, 1, 0, 100, 50);
            TextBoxActiveXControl activeXControl = (TextBoxActiveXControl)shape.ActiveXControl;

            // ضبط الخصائص
            activeXControl.BorderStyle = ControlBorderType.Single;
            activeXControl.BorderOleColor = unchecked((int)0x80000012); // Excel default color system 12 or green(0x0000FF00)
            activeXControl.SpecialEffect = ControlSpecialEffectType.Bump;
            if (activeXControl.MaxLength == 0)
            {
                activeXControl.MaxLength = 30;
            }
            activeXControl.ScrollBars = ControlScrollBarType.BarsVertical;
            activeXControl.PasswordChar = 'a';
            if (!activeXControl.IsEditable)
            {
                activeXControl.IsEditable = true;
            }
            if (!activeXControl.IntegralHeight)
            {
                activeXControl.IntegralHeight = true;
            }
            if (!activeXControl.IsDragBehaviorEnabled)
            {
                activeXControl.IsDragBehaviorEnabled = true;
            }
            if (!activeXControl.EnterKeyBehavior)
            {
                activeXControl.EnterKeyBehavior = true;
            }
            if (!activeXControl.EnterFieldBehavior)
            {
                activeXControl.EnterFieldBehavior = true;
            }
            if (!activeXControl.TabKeyBehavior)
            {
                activeXControl.TabKeyBehavior = true;
            }
            if (!activeXControl.HideSelection)
            {
                activeXControl.HideSelection = true;
            }
            if (!activeXControl.IsAutoTab)
            {
                activeXControl.IsAutoTab = true;
            }
            if (!activeXControl.IsMultiLine)
            {
                activeXControl.IsMultiLine = true;
            }
            if (!activeXControl.IsAutoWordSelected)
            {
                activeXControl.IsAutoWordSelected = true;
            }
            if (!activeXControl.IsWordWrapped)
            {
                activeXControl.IsWordWrapped = true;
            }
            activeXControl.Text = "This is a test.";
            activeXControl.DropButtonStyle = DropButtonStyle.Arrow;
            activeXControl.ShowDropButtonTypeWhen = ShowDropButtonType.Focus;

            // احفظ المصنف
            workbook.Save("TextBoxActiveXControlExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ActiveXControl](../activexcontrol/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


