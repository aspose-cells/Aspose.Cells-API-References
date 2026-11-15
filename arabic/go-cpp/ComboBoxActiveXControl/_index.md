---
title: "فئة ComboBoxActiveXControl"
linktitle: "ComboBoxActiveXControl"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة ComboBoxActiveXControl. تغلف الكائن الذي يمثل comboboxactivexcontrol في Go."
type: docs
weight: 200
url: /ar/go-cpp/comboboxactivexcontrol/
---

## ComboBoxActiveXControl class

يمثل عنصر التحكم ActiveX من نوع ComboBox.

```go

type ComboBoxActiveXControl struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewComboBoxActiveXControl](./newcomboboxactivexcontrol/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetType](./gettype/) | يحصل على نوع عنصر التحكم ActiveX. |
| [GetMaxLength](./getmaxlength/) | يحصل ويضبط الحد الأقصى لعدد الأحرف |
| [SetMaxLength](./setmaxlength/) | يحصل ويضبط الحد الأقصى لعدد الأحرف |
| [GetListWidth](./getlistwidth/) | يحصل ويضبط العرض بوحدة النقاط. |
| [SetListWidth](./setlistwidth/) | يحصل ويضبط العرض بوحدة النقاط. |
| [GetBoundColumn](./getboundcolumn/) | يمثل كيفية تحديد خاصية Value لـ ComboBox أو ListBox عندما تكون قيمة خاصية MultiSelect (fmMultiSelectSingle). |
| [SetBoundColumn](./setboundcolumn/) | يمثل كيفية تحديد خاصية Value لـ ComboBox أو ListBox عندما تكون قيمة خاصية MultiSelect (fmMultiSelectSingle). |
| [GetTextColumn](./gettextcolumn/) | يمثل العمود في ComboBox أو ListBox الذي يُعرض للمستخدم. |
| [SetTextColumn](./settextcolumn/) | يمثل العمود في ComboBox أو ListBox الذي يُعرض للمستخدم. |
| [GetColumnCount](./getcolumncount/) | يمثل عدد الأعمدة التي تُعرض في ComboBox أو ListBox. |
| [SetColumnCount](./setcolumncount/) | يمثل عدد الأعمدة التي تُعرض في ComboBox أو ListBox. |
| [GetListRows](./getlistrows/) | يمثل الحد الأقصى لعدد الصفوف التي تُعرض في القائمة. |
| [SetListRows](./setlistrows/) | يمثل الحد الأقصى لعدد الصفوف التي تُعرض في القائمة. |
| [GetMatchEntry](./getmatchentry/) | يشير إلى كيفية بحث ListBox أو ComboBox في قائمته أثناء كتابة المستخدم. |
| [SetMatchEntry](./setmatchentry/) | يشير إلى كيفية بحث ListBox أو ComboBox في قائمته أثناء كتابة المستخدم. |
| [GetDropButtonStyle](./getdropbuttonstyle/) | يحدد الرمز المعروض على زر السحب. |
| [SetDropButtonStyle](./setdropbuttonstyle/) | يحدد الرمز المعروض على زر السحب. |
| [GetShowDropButtonTypeWhen](./getshowdropbuttontypewhen/) | يحدد الرمز المعروض على زر السحب. |
| [SetShowDropButtonTypeWhen](./setshowdropbuttontypewhen/) | يحدد الرمز المعروض على زر السحب. |
| [GetListStyle](./getliststyle/) | يحصل ويضبط المظهر البصري. |
| [SetListStyle](./setliststyle/) | يحصل ويضبط المظهر البصري. |
| [GetBorderStyle](./getborderstyle/) | يحصل ويضبط نوع الحدود المستخدمة في التحكم. |
| [SetBorderStyle](./setborderstyle/) | يحصل ويضبط نوع الحدود المستخدمة في التحكم. |
| [GetBorderOleColor](./getborderolecolor/) | يحصل ويضبط لون OLE للخلفية. |
| [SetBorderOleColor](./setborderolecolor/) | يحصل ويضبط لون OLE للخلفية. |
| [GetSpecialEffect](./getspecialeffect/) | يحصل ويضبط التأثير الخاص بالتحكم. |
| [SetSpecialEffect](./setspecialeffect/) | يحصل ويضبط التأثير الخاص بالتحكم. |
| [IsEditable](./iseditable/) | يشير إلى ما إذا كان المستخدم يمكنه الكتابة في التحكم. |
| [SetIsEditable](./setiseditable/) | يشير إلى ما إذا كان المستخدم يمكنه الكتابة في التحكم. |
| [GetShowColumnHeads](./getshowcolumnheads/) | يشير إلى ما إذا كانت عناوين الأعمدة معروضة. |
| [SetShowColumnHeads](./setshowcolumnheads/) | يشير إلى ما إذا كانت عناوين الأعمدة معروضة. |
| [IsDragBehaviorEnabled](./isdragbehaviorenabled/) | يشير إلى ما إذا كان السحب والإفلات مفعلاً للتحكم. |
| [SetIsDragBehaviorEnabled](./setisdragbehaviorenabled/) | يشير إلى ما إذا كان السحب والإفلات مفعلاً للتحكم. |
| [GetEnterFieldBehavior](./getenterfieldbehavior/) | يحدد سلوك الاختيار عند دخول التحكم. True يعني أن الاختيار يبقى دون تغيير منذ آخر مرة كان فيها التحكم نشطًا. False يعني أنه سيتم تحديد كل النص في التحكم عند دخول التحكم. |
| [SetEnterFieldBehavior](./setenterfieldbehavior/) | يحدد سلوك الاختيار عند دخول التحكم. True يعني أن الاختيار يبقى دون تغيير منذ آخر مرة كان فيها التحكم نشطًا. False يعني أنه سيتم تحديد كل النص في التحكم عند دخول التحكم. |
| [GetSelectionMargin](./getselectionmargin/) | يشير إلى ما إذا كان المستخدم يمكنه تحديد سطر من النص بالنقر في المنطقة إلى يسار النص. |
| [SetSelectionMargin](./setselectionmargin/) | يشير إلى ما إذا كان المستخدم يمكنه تحديد سطر من النص بالنقر في المنطقة إلى يسار النص. |
| [GetValue](./getvalue/) | يحصل ويضبط قيمة التحكم. |
| [SetValue](./setvalue/) | يحصل ويضبط قيمة التحكم. |
| [GetHideSelection](./gethideselection/) | يشير إلى ما إذا كان النص المحدد في التحكم يظهر مميزًا عندما لا يكون للتحكم التركيز. |
| [SetHideSelection](./sethideselection/) | يشير إلى ما إذا كان النص المحدد في التحكم يظهر مميزًا عندما لا يكون للتحكم التركيز. |
| [GetColumnWidths](./getcolumnwidths/) | يحصل ويضبط عرض العمود. |
| [SetColumnWidths](./setcolumnwidths/) | يحصل ويضبط عرض العمود. |
| [IsAutoWordSelected](./isautowordselected/) | يحدد الوحدة الأساسية المستخدمة لتوسيع الاختيار. True يعني أن الوحدة الأساسية هي حرف واحد. false يعني أن الوحدة الأساسية هي كلمة كاملة. |
| [SetIsAutoWordSelected](./setisautowordselected/) | يحدد الوحدة الأساسية المستخدمة لتوسيع الاختيار. True يعني أن الوحدة الأساسية هي حرف واحد. false يعني أن الوحدة الأساسية هي كلمة كاملة. |
| [IsEnabled](./isenabled/) | يشير إلى ما إذا كان التحكم يمكنه استلام التركيز والاستجابة للأحداث التي يولدها المستخدم. |
| [SetIsEnabled](./setisenabled/) | يشير إلى ما إذا كان التحكم يمكنه استلام التركيز والاستجابة للأحداث التي يولدها المستخدم. |
| [IsLocked](./islocked/) | يشير إلى ما إذا كانت البيانات في التحكم مقفلة للتحرير. |
| [SetIsLocked](./setislocked/) | يشير إلى ما إذا كانت البيانات في التحكم مقفلة للتحرير. |
| [IsTransparent](./istransparent/) | يشير إلى ما إذا كان التحكم شفافًا. |
| [SetIsTransparent](./setistransparent/) | يشير إلى ما إذا كان التحكم شفافًا. |
| [GetIMEMode](./getimemode/) | يحصل على ويضبط وضع التشغيل الافتراضي لمحرر طريقة الإدخال للعنصر عند استلامه للتركيز. |
| [SetIMEMode](./setimemode/) | يحصل على ويضبط وضع التشغيل الافتراضي لمحرر طريقة الإدخال للعنصر عند استلامه للتركيز. |
| [GetFont](./getfont/) | يمثل خط التحكم. |
| [GetTextAlign](./gettextalign/) | يمثل طريقة محاذاة النص المستخدم في التحكم. |
| [SetTextAlign](./settextalign/) | يمثل طريقة محاذاة النص المستخدم في التحكم. |
| [GetData](./getdata/) | يحصل ويضبط البيانات الثنائية للعنصر التحكم. |
| [IsAutoSize](./isautosize/) | يشير إلى ما إذا كان التحكم سيعيد حجمه تلقائيًا لعرض محتوياته بالكامل. |
| [SetIsAutoSize](./setisautosize/) | يشير إلى ما إذا كان التحكم سيعيد حجمه تلقائيًا لعرض محتوياته بالكامل. |
| [GetWorkbook](./getworkbook/) | يحصل على كائن Workbook. |
| [GetMouseIcon](./getmouseicon/) | يحصل ويضبط أيقونة مخصصة لعرضها كمؤشر الفأرة للعنصر التحكم. |
| [SetMouseIcon](./setmouseicon/) | يحصل ويضبط أيقونة مخصصة لعرضها كمؤشر الفأرة للعنصر التحكم. |
| [GetMousePointer](./getmousepointer/) | يحصل ويضبط نوع الأيقونة المعروضة كمؤشر الفأرة للعنصر التحكم. |
| [SetMousePointer](./setmousepointer/) | يحصل ويضبط نوع الأيقونة المعروضة كمؤشر الفأرة للعنصر التحكم. |
| [GetLinkedCell](./getlinkedcell/) | يحصل ويضبط الخلية المرتبطة. |
| [SetLinkedCell](./setlinkedcell/) | يحصل ويضبط الخلية المرتبطة. |
| [GetListFillRange](./getlistfillrange/) | يحصل ويضبط نطاق تعبئة القائمة. |
| [SetListFillRange](./setlistfillrange/) | يحصل ويضبط نطاق تعبئة القائمة. |
| [GetWidth](./getwidth/) | يحصل ويضبط عرض العنصر التحكم بوحدة النقاط. |
| [SetWidth](./setwidth/) | يحصل ويضبط عرض العنصر التحكم بوحدة النقاط. |
| [GetHeight](./getheight/) | يحصل ويضبط ارتفاع العنصر التحكم بوحدة النقاط. |
| [SetHeight](./setheight/) | يحصل ويضبط ارتفاع العنصر التحكم بوحدة النقاط. |
| [GetForeOleColor](./getforeolecolor/) | يحصل ويضبط لون OLE للمقدمة. |
| [SetForeOleColor](./setforeolecolor/) | يحصل ويضبط لون OLE للمقدمة. |
| [GetBackOleColor](./getbackolecolor/) | يحصل ويضبط لون OLE للخلفية. |
| [SetBackOleColor](./setbackolecolor/) | يحصل ويضبط لون OLE للخلفية. |
| [IsVisible](./isvisible/) | يشير إلى ما إذا كان هذا العنصر التحكم مرئيًا. |
| [SetIsVisible](./setisvisible/) | يشير إلى ما إذا كان هذا العنصر التحكم مرئيًا. |
| [GetShadow](./getshadow/) | يشير إلى ما إذا كان يجب إظهار ظل. |
| [SetShadow](./setshadow/) | يشير إلى ما إذا كان يجب إظهار ظل. |
