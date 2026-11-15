---
title: "فئة CellsHelper"
linktitle: "CellsHelper"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة CellsHelper. تغلف الكائن الذي يمثل cellshelper في Go."
type: docs
weight: 200
url: /ar/go-cpp/cellshelper/
---

## CellsHelper class

يوفر وظائف مساعدة.

```go

type CellsHelper struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |

## طرق

| طريقة | الوصف |
| --- | --- |
| [CellsHelper_GetSignificantDigitsType](./cellshelper_getsignificantdigitstype/) | يحصل ويضبط النوع الافتراضي للأرقام ذات الأهمية عند إخراج القيم الرقمية. القيمة الافتراضية هي SignificantDigitsType.G17. |
| [CellsHelper_SetSignificantDigitsType](./cellshelper_setsignificantdigitstype/) | يحصل ويضبط النوع الافتراضي للأرقام ذات الأهمية عند إخراج القيم الرقمية. القيمة الافتراضية هي SignificantDigitsType.G17. |
| [CellsHelper_GetDPI](./cellshelper_getdpi/) | يحصل على DPI للجهاز. |
| [CellsHelper_SetDPI](./cellshelper_setdpi/) | يحصل على DPI للجهاز. |
| [CellsHelper_GetTextWidth](./cellshelper_gettextwidth/) | احصل على عرض النص بوحدة النقاط. |
| [CellsHelper_GetVersion](./cellshelper_getversion/) | احصل على نسخة الإصدار. |
| [CellsHelper_CellNameToIndex](./cellshelper_cellnametoindex/) | يحصل على فهارس الصف والعمود للخلية وفقًا لاسمها. |
| [CellsHelper_CellIndexToName](./cellshelper_cellindextoname/) | يحصل على اسم الخلية وفقًا لفهارس الصف والعمود. |
| [CellsHelper_ColumnIndexToName](./cellshelper_columnindextoname/) | يحصل على اسم العمود وفقًا لفهرس العمود. |
| [CellsHelper_ColumnNameToIndex](./cellshelper_columnnametoindex/) | يحصل على فهرس العمود وفقًا لاسم العمود. |
| [CellsHelper_RowIndexToName](./cellshelper_rowindextoname/) | يحصل على اسم الصف وفقًا لفهرس الصف. |
| [CellsHelper_RowNameToIndex](./cellshelper_rownametoindex/) | يحصل على فهرس الصف وفقًا لاسم الصف. |
| [CellsHelper_GetDateTimeFromDouble](./cellshelper_getdatetimefromdouble/) | حوّل القيمة المزدوجة إلى قيمة تاريخ ووقت. |
| [CellsHelper_GetDoubleFromDateTime](./cellshelper_getdoublefromdatetime/) | حوّل التاريخ والوقت إلى قيمة مزدوجة. |
| [CellsHelper_GetStartupPath](./cellshelper_getstartuppath/) | يحصل أو يضبط مسار بدء التشغيل، الذي يُشار إليه من قبل بعض مراجع الصيغ الخارجية. |
| [CellsHelper_SetStartupPath](./cellshelper_setstartuppath/) | يحصل أو يضبط مسار بدء التشغيل، الذي يُشار إليه من قبل بعض مراجع الصيغ الخارجية. |
| [CellsHelper_GetAltStartPath](./cellshelper_getaltstartpath/) | يحصل أو يضبط مسار بدء التشغيل البديل، الذي يُشار إليه من قبل بعض مراجع الصيغ الخارجية. |
| [CellsHelper_SetAltStartPath](./cellshelper_setaltstartpath/) | يحصل أو يضبط مسار بدء التشغيل البديل، الذي يُشار إليه من قبل بعض مراجع الصيغ الخارجية. |
| [CellsHelper_GetLibraryPath](./cellshelper_getlibrarypath/) | يحصل أو يضبط مسار المكتبة الذي يُشار إليه من قبل بعض مراجع الصيغ الخارجية. |
| [CellsHelper_SetLibraryPath](./cellshelper_setlibrarypath/) | يحصل أو يضبط مسار المكتبة الذي يُشار إليه من قبل بعض مراجع الصيغ الخارجية. |
| [CellsHelper_GetUsedColors](./cellshelper_getusedcolors/) | يحصل على جميع الألوان المستخدمة في دفتر العمل. |
| [CellsHelper_MergeFiles](./cellshelper_mergefiles/) | يدمج بعض ملفات xls الكبيرة إلى ملف xls واحد. |
| [CellsHelper_GetCacheFolder](./cellshelper_getcachefolder/) | يحصل على المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات. |
| [CellsHelper_SetCacheFolder](./cellshelper_setcachefolder/) | يضبط المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات. |
| [CellsHelper_CreateSafeSheetName_String](./cellshelper_createsafesheetname_string/) | يتحقق من اسم الورقة المُعطى وينشئ اسمًا صالحًا عند الحاجة. إذا كان اسم الورقة المُعطى يتوافق مع قواعد أسماء أوراق Excel، يتم إرجاعه. وإلا سيتم قطع السلسلة إذا تجاوز الطول الحد وسيتم استبدال الأحرف غير الصالحة بـ ' ', ثم إرجاع قيمة السلسلة المعاد بناؤها. |
| [CellsHelper_CreateSafeSheetName_String_Char](./cellshelper_createsafesheetname_string_char/) | يتحقق من اسم الورقة المُعطى وينشئ اسمًا صالحًا عند الحاجة. إذا كان اسم الورقة المُعطى يتوافق مع قواعد أسماء أوراق Excel، يتم إرجاعه. وإلا سيتم قطع السلسلة إذا تجاوز الطول الحد وسيتم استبدال الأحرف غير الصالحة بالحرف المُعطى، ثم إرجاع قيمة السلسلة المعاد بناؤها. |
| [CellsHelper_NeedQuoteInFormula](./cellshelper_needquoteinformula/) | يشير إلى ما إذا كان يجب إحاطة اسم الورقة بعلامات اقتباس مفردة |
| [CellsHelper_IsCloudPlatform](./cellshelper_iscloudplatform/) | يرجى ضبط هذه الخاصية إلى True عند التشغيل على منصة سحابية، مثل: Azure، AWSLambda، إلخ، |
| [CellsHelper_SetIsCloudPlatform](./cellshelper_setiscloudplatform/) | يرجى ضبط هذه الخاصية إلى True عند التشغيل على منصة سحابية، مثل: Azure، AWSLambda، إلخ، |
