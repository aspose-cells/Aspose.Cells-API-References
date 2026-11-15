---
title: "فئة Row"
linktitle: "Row"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة Row. تغلف الكائن الذي يمثل row في Go."
type: docs
weight: 200
url: /ar/go-cpp/row/
---

## Row class

يمثل صفًا واحدًا في ورقة العمل.

```go

type Row struct  {
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
| [GetCellByIndex](./getcellbyindex/) | احصل على الخلية بواسطة الفهرس المحدد في مجموعة الخلايا لهذا الصف. |
| [IsBlank](./isblank/) | يشير إلى ما إذا كان الصف يحتوي على أي بيانات |
| [Get](./get/) | يحصل على الخلية. |
| [GetEnumerator](./getenumerator/) | يحصل على عداد الخلايا |
| [GetEnumerator_Bool_Bool](./getenumerator_bool_bool/) | يحصل على عداد يتنقل عبر الخلايا في هذا الصف. |
| [GetCellOrNull](./getcellornull/) | يحصل على الخلية أو null في الفهرس المحدد. |
| [IsCollapsed](./iscollapsed/) | ما إذا كان الصف مطويًا |
| [SetIsCollapsed](./setiscollapsed/) | ما إذا كان الصف مطويًا |
| [GetHeight](./getheight/) | يحصل على ارتفاع الصف ويضبطه بوحدة النقاط. |
| [SetHeight](./setheight/) | يحصل على ارتفاع الصف ويضبطه بوحدة النقاط. |
| [IsHidden](./ishidden/) | يشير إلى ما إذا كان الصف مخفيًا. |
| [SetIsHidden](./setishidden/) | يشير إلى ما إذا كان الصف مخفيًا. |
| [GetIndex](./getindex/) | يحصل على فهرس هذا الصف. |
| [GetGroupLevel](./getgrouplevel/) | يحصل على مستوى المجموعة للصف. |
| [SetGroupLevel](./setgrouplevel/) | يحصل على مستوى المجموعة للصف. |
| [IsHeightMatched](./isheightmatched/) | يشير إلى ما إذا كان ارتفاع الصف يتطابق مع إعداد الخط الافتراضي الحالي لدفتر العمل. قيمة true لهذه الخاصية تعني أيضًا أن ارتفاع الصف "تلقائي" دون قيمة ارتفاع مخصصة تم تعيينها من قبل المستخدم. |
| [SetIsHeightMatched](./setisheightmatched/) | يشير إلى ما إذا كان ارتفاع الصف يتطابق مع إعداد الخط الافتراضي الحالي لدفتر العمل. قيمة true لهذه الخاصية تعني أيضًا أن ارتفاع الصف "تلقائي" دون قيمة ارتفاع مخصصة تم تعيينها من قبل المستخدم. |
| [GetStyle](./getstyle/) | يحصل على نمط هذا الصف. |
| [SetStyle](./setstyle/) | يضبط نمط هذا الصف. |
| [GetHasCustomStyle](./gethascustomstyle/) | يشير إلى ما إذا كان لهذا الصف إعدادات نمط مخصصة (مختلفة عن الإعداد الافتراضي الموروث من دفتر العمل). |
| [CopySettings](./copysettings/) | نسخ إعدادات الصف، مثل النمط، الارتفاع، الظهور، ... إلخ. |
| [GetFirstCell](./getfirstcell/) | يحصل على أول كائن خلية في الصف. |
| [GetFirstDataCell](./getfirstdatacell/) | يحصل على أول خلية غير فارغة في الصف. |
| [GetLastCell](./getlastcell/) | يحصل على آخر كائن خلية في الصف. |
| [GetLastDataCell](./getlastdatacell/) | يحصل على آخر خلية غير فارغة في الصف. |
| [ApplyStyle](./applystyle/) | يطبق التنسيقات على صف كامل. |
| [Equals_Object](./equals_object/) | يتحقق مما إذا كان هذا الكائن يشير إلى نفس الصف مع آخر. |
| [Equals_Row](./equals_row/) | يتحقق مما إذا كان هذا الكائن يشير إلى نفس الصف مع كائن صف آخر. |
