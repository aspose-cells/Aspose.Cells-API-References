---
title: "فئة Comment"
linktitle: "Comment"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة التعليق. تغلف الكائن الذي يمثل التعليق في Go."
type: docs
weight: 200
url: /ar/go-cpp/comment/
---

## Comment class

يغلف الكائن الذي يمثل تعليق خلية.

```go

type Comment struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetAuthor](./getauthor/) | يحصل ويضبط اسم مؤلف التعليق الأصلي |
| [SetAuthor](./setauthor/) | يحصل ويضبط اسم مؤلف التعليق الأصلي |
| [GetCommentShape](./getcommentshape/) | احصل على كائن Shape الذي يمثل الشكل المرفق بالتعليق المحدد. |
| [GetRow](./getrow/) | يحصل على فهرس الصف للتعليق. |
| [GetColumn](./getcolumn/) | يحصل على فهرس العمود للتعليق. |
| [IsThreadedComment](./isthreadedcomment/) | يشير إلى ما إذا كان هذا التعليق تعليقًا متسلسلًا. |
| [GetThreadedComments](./getthreadedcomments/) | يحصل على قائمة التعليقات المتسلسلة؛ |
| [GetNote](./getnote/) | يمثل محتوى التعليق. |
| [SetNote](./setnote/) | يمثل محتوى التعليق. |
| [GetHtmlNote](./gethtmlnote/) | يحصل ويضبط سلسلة html التي تحتوي على البيانات وبعض الصيغ في هذا التعليق. |
| [SetHtmlNote](./sethtmlnote/) | يحصل ويضبط سلسلة html التي تحتوي على البيانات وبعض الصيغ في هذا التعليق. |
| [GetFont](./getfont/) | يحصل على خط التعليق. |
| [FormatCharacters](./formatcharacters/) | نسق بعض الأحرف باستخدام إعداد الخط. |
| [Characters](./characters/) | يرجع كائن Characters الذي يمثل نطاقًا من الأحرف داخل نص التعليق. |
| [GetRichFormattings](./getrichformattings/) | يرجع جميع كائنات Characters التي تمثل نطاقًا من الأحرف داخل نص التعليق. |
| [IsVisible](./isvisible/) | يمثل ما إذا كان التعليق مرئيًا أم لا. |
| [SetIsVisible](./setisvisible/) | يمثل ما إذا كان التعليق مرئيًا أم لا. |
| [GetTextOrientationType](./gettextorientationtype/) | يحصل ويضبط نوع توجيه النص للتعليق. |
| [SetTextOrientationType](./settextorientationtype/) | يحصل ويضبط نوع توجيه النص للتعليق. |
| [GetTextHorizontalAlignment](./gettexthorizontalalignment/) | يحصل ويضبط نوع محاذاة النص الأفقية للتعليق. |
| [SetTextHorizontalAlignment](./settexthorizontalalignment/) | يحصل ويضبط نوع محاذاة النص الأفقية للتعليق. |
| [GetTextVerticalAlignment](./gettextverticalalignment/) | يحصل ويضبط نوع محاذاة النص العمودية للتعليق. |
| [SetTextVerticalAlignment](./settextverticalalignment/) | يحصل ويضبط نوع محاذاة النص العمودية للتعليق. |
| [GetAutoSize](./getautosize/) | يشير إلى ما إذا كان حجم التعليق يتم ضبطه تلقائيًا وفقًا لمحتواه. ملاحظة: في بعض الحالات الخاصة (مثل بيئة Mac)، قد لا يعمل هذا الإعداد. إذا لم يعمل هذا الإعداد، يرجى استبداله بـ FitToTextSize(). |
| [SetAutoSize](./setautosize/) | يشير إلى ما إذا كان حجم التعليق يتم ضبطه تلقائيًا وفقًا لمحتواه. ملاحظة: في بعض الحالات الخاصة (مثل بيئة Mac)، قد لا يعمل هذا الإعداد. إذا لم يعمل هذا الإعداد، يرجى استبداله بـ FitToTextSize(). |
| [GetHeightCM](./getheightcm/) | يمثل ارتفاع التعليق، بوحدة السنتيمترات. |
| [SetHeightCM](./setheightcm/) | يمثل ارتفاع التعليق، بوحدة السنتيمترات. |
| [GetWidthCM](./getwidthcm/) | يمثل عرض التعليق، بوحدة السنتيمترات. |
| [SetWidthCM](./setwidthcm/) | يمثل عرض التعليق، بوحدة السنتيمترات. |
| [GetWidth](./getwidth/) | يمثل عرض التعليق، بوحدة البكسل. |
| [SetWidth](./setwidth/) | يمثل عرض التعليق، بوحدة البكسل. |
| [GetHeight](./getheight/) | يمثل ارتفاع التعليق، بوحدة البكسل. |
| [SetHeight](./setheight/) | يمثل ارتفاع التعليق، بوحدة البكسل. |
| [GetWidthInch](./getwidthinch/) | يمثل عرض التعليق، بوحدة الإنش. |
| [SetWidthInch](./setwidthinch/) | يمثل عرض التعليق، بوحدة الإنش. |
| [GetHeightInch](./getheightinch/) | يمثل ارتفاع التعليق، بوحدة الإنش. |
| [SetHeightInch](./setheightinch/) | يمثل ارتفاع التعليق، بوحدة الإنش. |
