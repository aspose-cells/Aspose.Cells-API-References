---
title: "الفئة ComboBoxActiveXControl"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl. تمثّل عنصر تحكم ActiveX من نوع ComboBox"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/
---
## ComboBoxActiveXControl class

يمثل عنصر تحكم ActiveX من نوع ComboBox.

```csharp
public class ComboBoxActiveXControl : ActiveXControl
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | يحصل ويضبط لون الـole للخلفية. (موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [BorderOleColor](../../aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/borderolecolor/) { get; set; } | يحصل ويضبط لون الـole للخلفية. |
| [BorderStyle](../../aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/borderstyle/) { get; set; } | يحصل ويضبط نوع الإطار المستخدم من قبل العنصر. |
| [BoundColumn](../../aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/boundcolumn/) { get; set; } | يمثّل كيفية تحديد خاصية Value لعنصر ComboBox أو ListBox عندما تكون قيمة خاصية MultiSelect هي (fmMultiSelectSingle). |
| [ColumnCount](../../aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/columncount/) { get; set; } | يمثّل عدد الأعمدة التي تُعرض في عنصر ComboBox أو ListBox. |
| [ColumnWidths](../../aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/columnwidths/) { get; set; } | يحصل ويضبط عرض العمود. |
| override [Data](../../aspose.cells.drawing.activexcontrols/activexcontrol/data/) { get; } | يحصل ويضبط البيانات الثنائية للعنصر. (موروث من [`ActiveXControl`](../activexcontrol/).) |
| [DropButtonStyle](../../aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/dropbuttonstyle/) { get; set; } | يحدد الرمز المعروض على زر السقوط |
| [EnterFieldBehavior](../../aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/enterfieldbehavior/) { get; set; } | يحدد سلوك الاختيار عند دخول العنصر. True يعني أن الاختيار يبقى دون تغيير منذ آخر مرة كان فيها العنصر نشطًا. False يعني أنه سيتم تحديد كل النص داخل العنصر عند الدخول إليه. |
| [Font](../../aspose.cells.drawing.activexcontrols/activexcontrol/font/) { get; } | يمثّل خط العنصر. (موروث من [`ActiveXControl`](../activexcontrol/).) |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/) { get; set; } | يحصل ويضبط لون الـole للمقدمة. (موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height/) { get; set; } | يحصل ويضبط ارتفاع العنصر بوحدة النقاط. (موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [HideSelection](../../aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/hideselection/) { get; set; } | يشير إلى ما إذا كان النص المحدد في العنصر يظهر مميزًا عندما لا يكون للعنصر تركيز. |
| [IMEMode](../../aspose.cells.drawing.activexcontrols/activexcontrol/imemode/) { get; set; } | يحصل ويضبط وضع التشغيل الافتراضي لمحرّر طريقة الإدخال للعنصر عند حصوله على التركيز. (موروث من [`ActiveXControl`](../activexcontrol/).) |
| virtual [IsAutoSize](../../aspose.cells.drawing.activexcontrols/activexcontrol/isautosize/) { get; set; } | يشير إلى ما إذا كان العنصر سيعيد حجمه تلقائيًا لعرض محتوياته بالكامل. (موروث من [`ActiveXControl`](../activexcontrol/).) |
| virtual [IsAutoWordSelected](../../aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/isautowordselected/) { get; set; } | يحدد الوحدة الأساسية المستخدمة لتوسيع الاختيار. True يعني أن الوحدة الأساسية هي حرف واحد. false يعني أن الوحدة الأساسية هي كلمة كاملة. |
| [IsDragBehaviorEnabled](../../aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/isdragbehaviorenabled/) { get; set; } | يشير إلى ما إذا كان السحب والإفلات مفعّلاً للعنصر. |
| [IsEditable](../../aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/iseditable/) { get; set; } | يشير إلى ما إذا كان المستخدم يستطيع الكتابة في العنصر. |
| [IsEnabled](../../aspose.cells.drawing.activexcontrols/activexcontrol/isenabled/) { get; set; } | يشير إلى ما إذا كان العنصر يمكنه استلام التركيز والاستجابة للأحداث التي يولدها المستخدم. (موروث من [`ActiveXControl`](../activexcontrol/).) |
| [IsLocked](../../aspose.cells.drawing.activexcontrols/activexcontrol/islocked/) { get; set; } | يشير إلى ما إذا كانت البيانات في العنصر مقفلة للتحرير. (موروث من [`ActiveXControl`](../activexcontrol/).) |
| [IsTransparent](../../aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/) { get; set; } | يشير إلى ما إذا كان التحكم شفافًا.(موروث من [`ActiveXControl`](../activexcontrol/).) |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/) { get; set; } | يشير إلى ما إذا كان هذا التحكم مرئيًا.(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | يحصل على الخلية المرتبطة ويضبطها.(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | يحصل على نطاق تعبئة القائمة ويضبطه.(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ListRows](../../aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/listrows/) { get; set; } | يمثل الحد الأقصى لعدد الصفوف التي يتم عرضها في القائمة. |
| [ListStyle](../../aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/liststyle/) { get; set; } | يحصل على المظهر البصري ويضبطه. |
| [ListWidth](../../aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/listwidth/) { get; set; } | يحصل على العرض بوحدة النقاط ويضبطه. |
| [MatchEntry](../../aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/matchentry/) { get; set; } | يشير إلى كيفية بحث ListBox أو ComboBox في قائمته عندما يكتب المستخدم. |
| [MaxLength](../../aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/maxlength/) { get; set; } | يحصل على الحد الأقصى لعدد الأحرف ويضبطه |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | يحصل على أيقونة مخصصة لعرضها كمؤشر الفأرة للتحكم ويضبطها.(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | يحصل على نوع الأيقونة المعروضة كمؤشر الفأرة للتحكم ويضبطه.(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [SelectionMargin](../../aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/selectionmargin/) { get; set; } | يشير إلى ما إذا كان المستخدم يمكنه تحديد سطر من النص بالنقر في المنطقة إلى يسار النص. |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | يشير إلى ما إذا كان يجب إظهار ظل.(موروث من [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ShowColumnHeads](../../aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/showcolumnheads/) { get; set; } | يشير إلى ما إذا كانت عناوين الأعمدة معروضة. |
| [ShowDropButtonTypeWhen](../../aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/showdropbuttontypewhen/) { get; set; } | يحدد الرمز المعروض على زر السقوط |
| [SpecialEffect](../../aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/specialeffect/) { get; set; } | يحصل على التأثير الخاص للتحكم ويضبطه. |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | يمثل طريقة محاذاة النص المستخدم في التحكم.(موروث من [`ActiveXControl`](../activexcontrol/).) |
| [TextColumn](../../aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/textcolumn/) { get; set; } | يمثل العمود في ComboBox أو ListBox الذي يُعرض للمستخدم. |
| override [Type](../../aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/type/) { get; } | يحصل على نوع عنصر التحكم ActiveX. |
| [Value](../../aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/value/) { get; set; } | يحصل على قيمة التحكم ويضبطها. |
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
    public class ActiveXControlsClassComboBoxActiveXControlDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر تحكم ComboBox ActiveX إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 1, 1, 0, 0, 100, 30);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // حدد الخصائص لـ ComboBox
            comboBox.ListFillRange = "A1:A3";
            comboBox.LinkedCell = "B1";
            
            // أضف عناصر إلى ComboBox عن طريق تعبئة الخلايا في النطاق
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // حدد القيمة الأولية
            comboBox.Value = "Item 2";

            // احفظ المصنف
            workbook.Save("ComboBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ActiveXControl](../activexcontrol/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


