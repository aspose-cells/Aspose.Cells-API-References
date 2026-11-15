---
title: "فئة SplitPartInfo"
linktitle: "SplitPartInfo"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة SplitPartInfo. تغلف الكائن الذي يمثل splitpartinfo في Go."
type: docs
weight: 200
url: /ar/go-cpp/splitpartinfo/
---

## SplitPartInfo class

يمثل معلومات إدخال/إخراج واحد للعديد من الإدخالات/الإخراجات، مثل الصفحة الحالية التي سيتم عرضها عند تحويل جدول البيانات إلى صورة.

```go

type SplitPartInfo struct  {
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
| [GetPartIndex](./getpartindex/) | فهرس الجزء الحالي في التسلسل (بدءًا من 0). -1 يعني أنه لا توجد أجزاء متعددة لذا النتيجة واحدة. |
| [GetSheetIndex](./getsheetindex/) | فهرس الورقة التي يوجد فيها الجزء الحالي. -1 يدل على وجود ورقة واحدة فقط. |
| [GetSheetName](./getsheetname/) | اسم الورقة التي يوجد فيها الجزء الحالي. |
