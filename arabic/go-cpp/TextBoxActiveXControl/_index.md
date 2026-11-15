---
title: "TextBoxActiveXControl فئة"
linktitle: "TextBoxActiveXControl"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "TextBoxActiveXControl فئة. يحتوي على الكائن الذي يمثل textboxactivexcontrol في Go."
type: docs
weight: 200
url: /ar/go-cpp/textboxactivexcontrol/
---

## TextBoxActiveXControl class

يمثل عنصر تحكم ActiveX لصندوق النص.

```go

type TextBoxActiveXControl struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewTextBoxActiveXControl](./newtextboxactivexcontrol/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetType](./gettype/) | يحصل على نوع عنصر التحكم ActiveX. |
| [GetBorderStyle](./getborderstyle/) | يحصل ويضبط نوع الحدود المستخدمة في التحكم. |
| [SetBorderStyle](./setborderstyle/) | يحصل ويضبط نوع الحدود المستخدمة في التحكم. |
| [GetBorderOleColor](./getborderolecolor/) | يحصل ويضبط لون OLE للخلفية. |
| [SetBorderOleColor](./setborderolecolor/) | يحصل ويضبط لون OLE للخلفية. |
| [GetSpecialEffect](./getspecialeffect/) | يحصل ويضبط التأثير الخاص بالتحكم. |
| [SetSpecialEffect](./setspecialeffect/) | يحصل ويضبط التأثير الخاص بالتحكم. |
| [GetMaxLength](./getmaxlength/) | يحصل ويضبط الحد الأقصى لعدد الأحرف |
| [SetMaxLength](./setmaxlength/) | يحصل ويضبط الحد الأقصى لعدد الأحرف |
| [GetScrollBars](./getscrollbars/) | يشير إلى ما إذا كان التحكم يحتوي على أشرطة تمرير عمودية، أشرطة تمرير أفقية، كليهما، أو لا شيء. |
| [SetScrollBars](./setscrollbars/) | يشير إلى ما إذا كان التحكم يحتوي على أشرطة تمرير عمودية، أشرطة تمرير أفقية، كليهما، أو لا شيء. |
| [GetPasswordChar](./getpasswordchar/) | يحصل على ويضبط حرفًا يتم عرضه بدلاً من الأحرف التي تم إدخالها. |
| [SetPasswordChar](./setpasswordchar/) | يحصل على ويضبط حرفًا يتم عرضه بدلاً من الأحرف التي تم إدخالها. |
| [IsEditable](./iseditable/) | يشير إلى ما إذا كان المستخدم يمكنه الكتابة في التحكم. |
| [SetIsEditable](./setiseditable/) | يشير إلى ما إذا كان المستخدم يمكنه الكتابة في التحكم. |
| [GetIntegralHeight](./getintegralheight/) | يشير إلى ما إذا كان التحكم سيظهر فقط الأسطر الكاملة من النص دون إظهار أي أسطر جزئية. |
| [SetIntegralHeight](./setintegralheight/) | يشير إلى ما إذا كان التحكم سيظهر فقط الأسطر الكاملة من النص دون إظهار أي أسطر جزئية. |
| [IsDragBehaviorEnabled](./isdragbehaviorenabled/) | يشير إلى ما إذا كان السحب والإفلات مفعلاً للتحكم. |
| [SetIsDragBehaviorEnabled](./setisdragbehaviorenabled/) | يشير إلى ما إذا كان السحب والإفلات مفعلاً للتحكم. |
| [GetEnterKeyBehavior](./getenterkeybehavior/) | يحدد سلوك مفتاح ENTER. True يعني أن الضغط على ENTER سيُنشئ سطرًا جديدًا. False يعني أن الضغط على ENTER سينقل التركيز إلى العنصر التالي في ترتيب التبويب. |
| [SetEnterKeyBehavior](./setenterkeybehavior/) | يحدد سلوك مفتاح ENTER. True يعني أن الضغط على ENTER سيُنشئ سطرًا جديدًا. False يعني أن الضغط على ENTER سينقل التركيز إلى العنصر التالي في ترتيب التبويب. |
| [GetEnterFieldBehavior](./getenterfieldbehavior/) | يحدد سلوك الاختيار عند دخول التحكم. True يعني أن الاختيار يبقى دون تغيير منذ آخر مرة كان فيها التحكم نشطًا. False يعني أنه سيتم تحديد كل النص في التحكم عند دخول التحكم. |
| [SetEnterFieldBehavior](./setenterfieldbehavior/) | يحدد سلوك الاختيار عند دخول التحكم. True يعني أن الاختيار يبقى دون تغيير منذ آخر مرة كان فيها التحكم نشطًا. False يعني أنه سيتم تحديد كل النص في التحكم عند دخول التحكم. |
| [GetTabKeyBehavior](./gettabkeybehavior/) | يشير إلى ما إذا كان يُسمح بأحرف الجدولة في نص التحكم. |
| [SetTabKeyBehavior](./settabkeybehavior/) | يشير إلى ما إذا كان يُسمح بأحرف الجدولة في نص التحكم. |
| [GetHideSelection](./gethideselection/) | يشير إلى ما إذا كان النص المحدد في التحكم يظهر مميزًا عندما لا يكون للتحكم التركيز. |
| [SetHideSelection](./sethideselection/) | يشير إلى ما إذا كان النص المحدد في التحكم يظهر مميزًا عندما لا يكون للتحكم التركيز. |
| [IsAutoTab](./isautotab/) | يشير إلى ما إذا كان سيُنتقل التركيز تلقائيًا إلى التحكم التالي عندما يُدخل المستخدم الحد الأقصى لعدد الأحرف. |
| [SetIsAutoTab](./setisautotab/) | يشير إلى ما إذا كان سيُنتقل التركيز تلقائيًا إلى التحكم التالي عندما يُدخل المستخدم الحد الأقصى لعدد الأحرف. |
| [IsMultiLine](./ismultiline/) | يشير إلى ما إذا كان التحكم يمكنه عرض أكثر من سطر نص واحد. |
| [SetIsMultiLine](./setismultiline/) | يشير إلى ما إذا كان التحكم يمكنه عرض أكثر من سطر نص واحد. |
| [IsWordWrapped](./iswordwrapped/) | يشير إلى ما إذا كان محتوى عنصر التحكم يلتف تلقائيًا في نهاية السطر. |
| [SetIsWordWrapped](./setiswordwrapped/) | يشير إلى ما إذا كان محتوى عنصر التحكم يلتف تلقائيًا في نهاية السطر. |
| [GetText](./gettext/) | يحصل على ويضبط نص التحكم. |
| [SetText](./settext/) | يحصل على ويضبط نص التحكم. |
| [GetDropButtonStyle](./getdropbuttonstyle/) | يحدد الرمز المعروض على زر السحب. |
| [SetDropButtonStyle](./setdropbuttonstyle/) | يحدد الرمز المعروض على زر السحب. |
| [GetShowDropButtonTypeWhen](./getshowdropbuttontypewhen/) | يحدد الرمز المعروض على زر السحب. |
| [SetShowDropButtonTypeWhen](./setshowdropbuttontypewhen/) | يحدد الرمز المعروض على زر السحب. |
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
