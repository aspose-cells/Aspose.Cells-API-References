---
title: "DataBar فئة"
linktitle: "DataBar"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "DataBar فئة. يغلف الكائن الذي يمثل databar في Go."
type: docs
weight: 200
url: /ar/go-cpp/databar/
---

## DataBar class

وصف قاعدة تنسيق الشرطية DataBar. تعرض قاعدة التنسيق الشرطي هذه شريط بيانات متدرج في نطاق الخلايا.

```go

type DataBar struct  {
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
| [GetAxisColor](./getaxiscolor/) | يحصل على لون المحور للخلايا ذات التنسيق الشرطي كأشرطة بيانات. |
| [SetAxisColor](./setaxiscolor/) | يحصل على لون المحور للخلايا ذات التنسيق الشرطي كأشرطة بيانات. |
| [GetAxisPosition](./getaxisposition/) | يحصل أو يضبط موضع محور أشرطة البيانات المحدد بواسطة قاعدة تنسيق شرطي. |
| [SetAxisPosition](./setaxisposition/) | يحصل أو يضبط موضع محور أشرطة البيانات المحدد بواسطة قاعدة تنسيق شرطي. |
| [GetBarFillType](./getbarfilltype/) | يحصل أو يضبط طريقة تعبئة شريط البيانات باللون. |
| [SetBarFillType](./setbarfilltype/) | يحصل أو يضبط طريقة تعبئة شريط البيانات باللون. |
| [GetDirection](./getdirection/) | يحصل أو يضبط اتجاه عرض شريط البيانات. |
| [SetDirection](./setdirection/) | يحصل أو يضبط اتجاه عرض شريط البيانات. |
| [GetBarBorder](./getbarborder/) | يحصل على كائن يحدد حدود شريط البيانات. |
| [GetNegativeBarFormat](./getnegativebarformat/) | يحصل على كائن NegativeBarFormat المرتبط بقاعدة تنسيق شرطي لشريط البيانات. |
| [GetMinCfvo](./getmincfvo/) | احصل أو اضبط كائن القيمة الدنيا لهذا DataBar. لا يمكن تعيين null أو CFValueObject من النوع FormatConditionValueType.Max إليه. |
| [GetMaxCfvo](./getmaxcfvo/) | احصل أو اضبط كائن القيمة القصوى لهذا DataBar. لا يمكن تعيين null أو CFValueObject من النوع FormatConditionValueType.Min إليه. |
| [GetColor](./getcolor/) | احصل أو اضبط لون هذا DataBar. |
| [SetColor](./setcolor/) | احصل أو اضبط لون هذا DataBar. |
| [GetMinLength](./getminlength/) | يمثل الحد الأدنى لطول شريط البيانات. |
| [SetMinLength](./setminlength/) | يمثل الحد الأدنى لطول شريط البيانات. |
| [GetMaxLength](./getmaxlength/) | يمثل الحد الأقصى لطول شريط البيانات. |
| [SetMaxLength](./setmaxlength/) | يمثل الحد الأقصى لطول شريط البيانات. |
| [GetShowValue](./getshowvalue/) | احصل أو اضبط العلامة التي تشير إلى ما إذا كان يجب إظهار قيم الخلايا التي يُطبق عليها هذا شريط البيانات. القيمة الافتراضية هي true. |
| [SetShowValue](./setshowvalue/) | احصل أو اضبط العلامة التي تشير إلى ما إذا كان يجب إظهار قيم الخلايا التي يُطبق عليها هذا شريط البيانات. القيمة الافتراضية هي true. |
| [ToImage](./toimage/) | تحويل شريط البيانات في الخلية إلى مصفوفة بايت للصورة. |
