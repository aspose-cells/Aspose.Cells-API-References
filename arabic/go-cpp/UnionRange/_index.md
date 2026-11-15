---
title: "فئة UnionRange"
linktitle: "UnionRange"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة UnionRange. تغلف الكائن الذي يمثل unionrange في Go."
type: docs
weight: 200
url: /ar/go-cpp/unionrange/
---

## UnionRange class

يمثل نطاق الاتحاد.

```go

type UnionRange struct  {
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
| [GetFirstRow](./getfirstrow/) | يحصل على فهرس الصف الأول للنطاق. |
| [GetFirstColumn](./getfirstcolumn/) | يحصل على فهرس العمود الأول للنطاق. |
| [GetRowCount](./getrowcount/) | يحصل على عدد الصفوف في النطاق. |
| [GetColumnCount](./getcolumncount/) | يحصل على عدد الصفوف في النطاق. |
| [Merge](./merge/) | يجمع مجموعة من الخلايا في خلية واحدة. |
| [UnMerge](./unmerge/) | يفك دمج الخلايا المدمجة في هذا النطاق. |
| [PutValue](./putvalue/) | يضع قيمة في النطاق، وإذا كان مناسبًا سيتم تحويل القيمة إلى نوع بيانات آخر وسيتم إعادة ضبط تنسيق الرقم للخلية. |
| [GetValue](./getvalue/) | يحصل على قيم النطاق ويضبطها. |
| [SetValue](./setvalue/) | يحصل على قيم النطاق ويضبطها. |
| [GetName](./getname/) | يحصل أو يضبط اسم النطاق. |
| [SetName](./setname/) | يحصل أو يضبط اسم النطاق. |
| [GetRefersTo](./getrefersto/) | يحصل على ما يشير إليه النطاق. |
| [GetHasRange](./gethasrange/) | يشير إلى ما إذا كان لهذا نطاق. |
| [GetHyperlinks](./gethyperlinks/) | يحصل على جميع الروابط التشعبية في النطاق. |
| [SetStyle](./setstyle/) | يضبط نمط النطاق. |
| [ApplyStyle](./applystyle/) | يطبق التنسيقات على النطاق بأكمله. |
| [Copy](./copy/) | نسخ النطاق باستخدام خيارات اللصق الخاصة. |
| [GetEnumerator](./getenumerator/) | يحصل على المُعدِّد للخلية في هذا النطاق. |
| [GetCellCount](./getcellcount/) | يحصل على عدد جميع الخلايا في النطاق. |
| [GetRangeCount](./getrangecount/) | يحصل على عدد النطاقات. |
| [GetRanges](./getranges/) | يحصل على جميع نطاقات الاتحاد. |
| [SetOutlineBorders_CellBorderTypeArray_ColorArray](./setoutlineborders_cellbordertypearray_colorarray/) | يضبط حدود الإطار حول مجموعة من الخلايا. |
| [SetOutlineBorders_CellBorderType_Color](./setoutlineborders_cellbordertype_color/) | يضبط حدود الإطار حول مجموعة من الخلايا بنفس نمط الحدود واللون. |
| [Intersect_String](./intersect_string/) | يتقاطع مع نطاق آخر. |
| [Intersect_UnionRange](./intersect_unionrange/) | يتقاطع مع نطاق آخر. |
| [Intersect_RangeArray](./intersect_rangearray/) | يتقاطع مع نطاق آخر. |
| [Union_String](./union_string/) | دمج نطاق آخر. |
| [Union_UnionRange](./union_unionrange/) | دمج نطاق آخر. |
| [Union_RangeArray](./union_rangearray/) | دمج النطاقات. |
