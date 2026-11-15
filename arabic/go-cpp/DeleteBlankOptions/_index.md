---
title: "DeleteBlankOptions فئة"
linktitle: "DeleteBlankOptions"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "DeleteBlankOptions class. يغلف الكائن الذي يمثل deleteblankoptions في Go."
type: docs
weight: 200
url: /ar/go-cpp/deleteblankoptions/
---

## DeleteBlankOptions class

يمثل إعداد حذف الخلايا/الصفوف/الأعمدة الفارغة.

```go

type DeleteBlankOptions struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewDeleteBlankOptions](./newdeleteblankoptions/) | البناء الافتراضي. |
| [NewDeleteBlankOptions_DeleteOptions](./newdeleteblankoptions_deleteoptions/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetEmptyStringAsBlank](./getemptystringasblank/) | يشير إلى ما إذا كان سيتم اعتبار خلية واحدة فارغة عندما تكون قيمتها سلسلة فارغة. القيمة الافتراضية هي true. |
| [SetEmptyStringAsBlank](./setemptystringasblank/) | يشير إلى ما إذا كان سيتم اعتبار خلية واحدة فارغة عندما تكون قيمتها سلسلة فارغة. القيمة الافتراضية هي true. |
| [GetEmptyFormulaValueAsBlank](./getemptyformulavalueasblank/) | ما إذا كان سيتم اعتبار خلية واحدة فارغة عندما تكون صيغة والنتيجة المحسوبة null أو سلسلة فارغة. القيمة الافتراضية هي false. |
| [SetEmptyFormulaValueAsBlank](./setemptyformulavalueasblank/) | ما إذا كان سيتم اعتبار خلية واحدة فارغة عندما تكون صيغة والنتيجة المحسوبة null أو سلسلة فارغة. القيمة الافتراضية هي false. |
| [GetDrawingsAsBlank](./getdrawingsasblank/) | يشير إلى ما إذا كانت الكائنات المتعلقة بالرسم مثل الصورة، الشكل، المخطط... سيتم اعتبارها فارغة. القيمة الافتراضية هي true. |
| [SetDrawingsAsBlank](./setdrawingsasblank/) | يشير إلى ما إذا كانت الكائنات المتعلقة بالرسم مثل الصورة، الشكل، المخطط... سيتم اعتبارها فارغة. القيمة الافتراضية هي true. |
| [GetMergedCellsShrinkType](./getmergedcellsshrinktype/) | يشير إلى كيفية معالجة الخلايا المدمجة عند حذف الصفوف/الأعمدة الفارغة. |
| [SetMergedCellsShrinkType](./setmergedcellsshrinktype/) | يشير إلى كيفية معالجة الخلايا المدمجة عند حذف الصفوف/الأعمدة الفارغة. |
| [GetStartIndex](./getstartindex/) | يحدد فهرس الصف/العمود الابتدائي للنطاق الذي يتم فحصه وحذف الصف/العمود الفارغ. |
| [SetStartIndex](./setstartindex/) | يحدد فهرس الصف/العمود الابتدائي للنطاق الذي يتم فحصه وحذف الصف/العمود الفارغ. |
| [GetEndIndex](./getendindex/) | يحدد فهرس الصف/العمود النهائي (شامل) للنطاق الذي يتم فحصه وحذف الصفوف/الأعمدة الفارغة. القيمة الافتراضية هي -1 و -1 تعني النطاق الأقصى لجميع الكائنات (الخلايا، الرسومات، ...) التي تحتاج إلى الفحص. |
| [SetEndIndex](./setendindex/) | يحدد فهرس الصف/العمود النهائي (شامل) للنطاق الذي يتم فحصه وحذف الصفوف/الأعمدة الفارغة. القيمة الافتراضية هي -1 و -1 تعني النطاق الأقصى لجميع الكائنات (الخلايا، الرسومات، ...) التي تحتاج إلى الفحص. |
| [GetUpdateReference](./getupdatereference/) | يشير إلى ما إذا كان يتم تحديث المراجع في أوراق عمل أخرى. |
| [SetUpdateReference](./setupdatereference/) | يشير إلى ما إذا كان يتم تحديث المراجع في أوراق عمل أخرى. |
| [GetFormulaChangeMonitor](./getformulachangemonitor/) | يحصل/يضبط المراقب لتتبع التغييرات الناجمة عن الحذف. |
| [SetFormulaChangeMonitor](./setformulachangemonitor/) | يحصل/يضبط المراقب لتتبع التغييرات الناجمة عن الحذف. |
