---
title: "فئة CheckBoxActiveXControl"
linktitle: "CheckBoxActiveXControl"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة CheckBoxActiveXControl. تغلف الكائن الذي يمثل checkboxactivexcontrol في لغة Go."
type: docs
weight: 200
url: /ar/go-cpp/checkboxactivexcontrol/
---

## CheckBoxActiveXControl class

يمثل عنصر التحكم ActiveX من نوع CheckBox.

```go

type CheckBoxActiveXControl struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewCheckBoxActiveXControl](./newcheckboxactivexcontrol/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetType](./gettype/) | يحصل على نوع عنصر التحكم ActiveX. |
| [GetGroupName](./getgroupname/) | يحصل على اسم المجموعة ويضبطه. |
| [SetGroupName](./setgroupname/) | يحصل على اسم المجموعة ويضبطه. |
| [GetAlignment](./getalignment/) | يحصل على موضع Caption بالنسبة للعنصر الضابط ويضبطه. |
| [SetAlignment](./setalignment/) | يحصل على موضع Caption بالنسبة للعنصر الضابط ويضبطه. |
| [IsWordWrapped](./iswordwrapped/) | يشير إلى ما إذا كان محتوى عنصر التحكم يلتف تلقائيًا في نهاية السطر. |
| [SetIsWordWrapped](./setiswordwrapped/) | يشير إلى ما إذا كان محتوى عنصر التحكم يلتف تلقائيًا في نهاية السطر. |
| [GetCaption](./getcaption/) | يسترجع ويضبط النص الوصفي الذي يظهر على عنصر التحكم. |
| [SetCaption](./setcaption/) | يسترجع ويضبط النص الوصفي الذي يظهر على عنصر التحكم. |
| [GetPicturePosition](./getpictureposition/) | يسترجع ويضبط موقع صورة عنصر التحكم بالنسبة إلى تسميته. |
| [SetPicturePosition](./setpictureposition/) | يسترجع ويضبط موقع صورة عنصر التحكم بالنسبة إلى تسميته. |
| [GetSpecialEffect](./getspecialeffect/) | يحصل ويضبط التأثير الخاص بالتحكم. |
| [SetSpecialEffect](./setspecialeffect/) | يحصل ويضبط التأثير الخاص بالتحكم. |
| [GetPicture](./getpicture/) | يسترجع ويضبط بيانات الصورة. |
| [SetPicture](./setpicture/) | يسترجع ويضبط بيانات الصورة. |
| [GetAccelerator](./getaccelerator/) | يسترجع ويضبط مفتاح الاختصار لعنصر التحكم. |
| [SetAccelerator](./setaccelerator/) | يسترجع ويضبط مفتاح الاختصار لعنصر التحكم. |
| [GetValue](./getvalue/) | يشير إلى ما إذا كان التحكم محددًا أم لا. |
| [SetValue](./setvalue/) | يشير إلى ما إذا كان التحكم محددًا أم لا. |
| [IsTripleState](./istriplestate/) | يشير إلى كيفية عرض القيم Null بواسطة التحكم المحدد. |
| [SetIsTripleState](./setistriplestate/) | يشير إلى كيفية عرض القيم Null بواسطة التحكم المحدد. |
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
