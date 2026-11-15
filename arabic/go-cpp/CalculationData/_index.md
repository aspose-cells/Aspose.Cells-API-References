---
title: "CalculationData فئة"
linktitle: "CalculationData"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة CalculationData. يغلف الكائن الذي يمثل calculationdata في Go."
type: docs
weight: 200
url: /ar/go-cpp/calculationdata/
---

## CalculationData class

يمثل البيانات المطلوبة عند حساب دالة واحدة، مثل اسم الدالة، المعلمات، ... إلخ.

```go

type CalculationData struct  {
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
| [GetCalculatedValue](./getcalculatedvalue/) | يحصل أو يضبط القيمة المحسوبة لهذه الدالة. |
| [SetCalculatedValue](./setcalculatedvalue/) | يحصل أو يضبط القيمة المحسوبة لهذه الدالة. |
| [GetWorkbook](./getworkbook/) | يحصل على كائن Workbook حيث توجد الدالة. |
| [GetWorksheet](./getworksheet/) | يحصل على كائن Worksheet حيث توجد الدالة. |
| [GetCellRow](./getcellrow/) | يحصل على فهرس الصف للخلية التي توجد فيها الدالة. |
| [GetCellColumn](./getcellcolumn/) | يحصل على فهرس العمود للخلية التي توجد فيها الدالة. |
| [GetCell](./getcell/) | يحصل على كائن Cell حيث توجد الدالة. |
| [GetFunctionName](./getfunctionname/) | يحصل على اسم الدالة التي سيتم حسابها. |
| [GetParamCount](./getparamcount/) | يحصل على عدد المعلمات |
| [GetParamValue](./getparamvalue/) | يحصل على كائن القيمة الممثلة للمعامل عند فهرس معين. |
| [GetParamValueInArrayMode](./getparamvalueinarraymode/) | يحصل على قيمة (القيم) المعامل عند فهرس معين. إذا كان المعامل نوعًا من التعبير الذي يحتاج إلى حساب، فسيتم حسابه في وضع المصفوفة. |
| [GetParamText](./getparamtext/) | يحصل على النص الحرفي للمعامل عند الفهرس المعطى. |
