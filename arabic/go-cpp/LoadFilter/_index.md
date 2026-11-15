---
title: "فئة LoadFilter"
linktitle: "LoadFilter"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة LoadFilter. يغلف الكائن الذي يمثل loadfilter في Go."
type: docs
weight: 200
url: /ar/go-cpp/loadfilter/
---

## LoadFilter class

يمثل الفلتر الذي يوفر خيارات لتحميل البيانات عند تحميل دفتر العمل من القالب.

```go

type LoadFilter struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewLoadFilter](./newloadfilter/) | ينشئ LoadFilter واحد مع خيارات الفلتر الافتراضية LoadDataFilterOptions::All. |
| [NewLoadFilter_LoadDataFilterOptions](./newloadfilter_loaddatafilteroptions/) | ينشئ LoadFilter واحد مع خيارات الفلتر المعطاة. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetLoadDataFilterOptions](./getloaddatafilteroptions/) | يحصل على خيارات الفلتر لتحديد البيانات التي يجب تحميلها. |
| [SetLoadDataFilterOptions](./setloaddatafilteroptions/) | يضبط خيارات الفلتر لتحديد البيانات التي يجب تحميلها. |
| [GetSheetsInLoadingOrder](./getsheetsinloadingorder/) | يحدد الأوراق (المؤشرات) والترتيب الذي سيتم تحميله. القيمة الافتراضية هي null، مما يعني تحميل جميع الأوراق بالترتيب الافتراضي في ملف القالب. إذا لم تكن null وكان مؤشر بعض الورق غير موجود في المصفوفة المعادة، فلن يتم تحميل ذلك الورق. |
| [StartSheet](./startsheet/) | يُعد خيارات الفلتر قبل تحميل ورقة العمل المحددة. يمكن لتطبيق المستخدم لـ LoadFilter تغيير LoadDataFilterOptions هنا لتحديد كيفية تحميل البيانات لهذه الورقة. |
