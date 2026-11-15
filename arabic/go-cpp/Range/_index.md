---
title: "فئة Range"
linktitle: "Range"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة Range. يغلف الكائن الذي يمثل range في Go."
type: docs
weight: 200
url: /ar/go-cpp/range/
---

## Range class

يغلف الكائن الذي يمثل نطاقًا من الخلايا داخل جدول بيانات.

```go

type Range struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewRange_CellArea_Cells](./newrange_cellarea_cells/) | منشئ الفئة. |
| [NewRange_Int_Int_Int_Int_Cells](./newrange_int_int_int_int_cells/) | منشئ الفئة. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [AutoFill_Range](./autofill_range/) | ملء النطاق المستهدف تلقائيًا. |
| [AutoFill_Range_AutoFillType](./autofill_range_autofilltype/) | ملء النطاق المستهدف تلقائيًا. |
| [GetCurrentRegion](./getcurrentregion/) | يرجع كائن Range يمثل المنطقة الحالية. المنطقة الحالية هي نطاق محاط بأي تركيبة من الصفوف الفارغة والأعمدة الفارغة. |
| [GetHyperlinks](./gethyperlinks/) | يحصل على جميع الروابط التشعبية في النطاق. |
| [AddHyperlink](./addhyperlink/) | يضيف رابطًا تشعبيًا إلى خلية محددة أو نطاق من الخلايا. |
| [GetEnumerator](./getenumerator/) | يحصل على المُعدِّد للخلية في هذا النطاق. |
| [IsIntersect](./isintersect/) | يشير إلى ما إذا كان النطاق يتقاطع. |
| [Intersect](./intersect/) | يرجع كائن Range يمثل تقاطعًا مستطيلًا بين نطاقين. |
| [UnionRanges](./unionranges/) | يرجع نتيجة الاتحاد بين نطاقين. |
| [GetRowCount](./getrowcount/) | يحصل على عدد الصفوف في النطاق. |
| [GetColumnCount](./getcolumncount/) | يحصل على عدد الأعمدة في النطاق. |
| [GetName](./getname/) | يحصل أو يضبط اسم النطاق. |
| [SetName](./setname/) | يحصل أو يضبط اسم النطاق. |
| [GetRefersTo](./getrefersto/) | يحصل على ما يشير إليه النطاق. |
| [GetAddress](./getaddress/) | يحصل على عنوان النطاق. |
| [IsBlank](./isblank/) | يشير إلى ما إذا كان النطاق يحتوي على قيم. |
| [GetLeft](./getleft/) | يحصل على المسافة، بالنقاط، من الحافة اليسرى للعمود A إلى الحافة اليسرى للنطاق. |
| [GetTop](./gettop/) | يحصل على المسافة، بالنقاط، من الحافة العلوية للصف 1 إلى الحافة العلوية للنطاق. |
| [GetWidth](./getwidth/) | يحصل على عرض النطاق بالنقاط. |
| [GetHeight](./getheight/) | يحصل على عرض النطاق بالنقاط. |
| [GetFirstRow](./getfirstrow/) | يحصل على فهرس الصف الأول للنطاق. |
| [GetFirstColumn](./getfirstcolumn/) | يحصل على فهرس العمود الأول للنطاق. |
| [Merge](./merge/) | يجمع مجموعة من الخلايا في خلية واحدة. |
| [UnMerge](./unmerge/) | يفك دمج الخلايا المدمجة في هذا النطاق. |
| [PutValue](./putvalue/) | يضع قيمة في النطاق، وإذا كان مناسبًا سيتم تحويل القيمة إلى نوع بيانات آخر وسيتم إعادة ضبط تنسيق الرقم للخلية. |
| [GetValue](./getvalue/) | يحصل على قيمة النطاق ويضبطها. |
| [SetValue](./setvalue/) | يحصل على قيمة النطاق ويضبطها. |
| [SetStyle_Style_Bool](./setstyle_style_bool/) | تطبيق نمط الخلية. |
| [ApplyStyle](./applystyle/) | يطبق التنسيقات على النطاق بأكمله. |
| [SetStyle_Style](./setstyle_style/) | يضبط نمط النطاق. |
| [SetOutlineBorders_CellBorderType_CellsColor](./setoutlineborders_cellbordertype_cellscolor/) | يضبط حدود الإطار حول مجموعة من الخلايا بنفس نمط الحدود واللون. |
| [SetOutlineBorders_CellBorderType_Color](./setoutlineborders_cellbordertype_color/) | يضبط حدود الإطار حول مجموعة من الخلايا بنفس نمط الحدود واللون. |
| [SetOutlineBorders_CellBorderTypeArray_ColorArray](./setoutlineborders_cellbordertypearray_colorarray/) | يضبط حدود الإطار حول مجموعة من الخلايا. |
| [SetOutlineBorder_BorderType_CellBorderType_CellsColor](./setoutlineborder_bordertype_cellbordertype_cellscolor/) | يضبط حد الإطار حول مجموعة من الخلايا. |
| [SetOutlineBorder_BorderType_CellBorderType_Color](./setoutlineborder_bordertype_cellbordertype_color/) | يضبط حد الإطار حول مجموعة من الخلايا. |
| [SetInsideBorders](./setinsideborders/) | يضبط الحدود الداخلية للنطاق. |
| [GetColumnWidth](./getcolumnwidth/) | يضبط أو يحصل على عرض العمود لهذا النطاق |
| [SetColumnWidth](./setcolumnwidth/) | يضبط أو يحصل على عرض العمود لهذا النطاق |
| [GetRowHeight](./getrowheight/) | يضبط أو يحصل على ارتفاع الصفوف في هذا النطاق |
| [SetRowHeight](./setrowheight/) | يضبط أو يحصل على ارتفاع الصفوف في هذا النطاق |
| [MoveTo](./moveto/) | نقل النطاق الحالي إلى النطاق الوجهة. |
| [CopyData](./copydata/) | ينسخ بيانات الخلية (بما في ذلك الصيغ) من نطاق المصدر. |
| [CopyValue](./copyvalue/) | ينسخ قيمة الخلية من نطاق المصدر. |
| [CopyStyle](./copystyle/) | ينسخ إعدادات النمط من نطاق المصدر. |
| [Copy_Range_PasteOptions](./copy_range_pasteoptions/) | نسخ النطاق باستخدام خيارات اللصق الخاصة. |
| [Transpose](./transpose/) | تحويل (تدوير) البيانات من الصفوف إلى الأعمدة أو العكس. |
| [Copy_Range](./copy_range/) | ينسخ البيانات (بما في ذلك الصيغ)، التنسيق، كائنات الرسم وغيرها من نطاق المصدر. |
| [Get](./get/) | يحصل على كائن Cell في هذا النطاق. |
| [GetCellOrNull](./getcellornull/) | يحصل على كائن Cell أو null في هذا النطاق. |
| [GetOffset](./getoffset/) | يحصل على نطاق Range بالإزاحة. |
| [GetEntireColumn](./getentirecolumn/) | يحصل على كائن Range الذي يمثل العمود (أو الأعمدة) بالكامل الذي يحتوي على النطاق المحدد. |
| [GetEntireRow](./getentirerow/) | يحصل على كائن Range الذي يمثل الصف (أو الصفوف) بالكامل الذي يحتوي على النطاق المحدد. |
| [GetWorksheet](./getworksheet/) | يحصل على كائن Worksheetobject الذي يحتوي على هذا النطاق. |
| [ToString](./tostring/) | يرجع سلسلة تمثل كائن Range الحالي. |
| [ToImage](./toimage/) | يحول النطاق إلى صورة. |
| [ToJson](./tojson/) | حول النطاق إلى قيمة JSON. |
| [ToHtml](./tohtml/) | حول النطاق إلى HTML. |
| [Clear](./clear/) | يمسح هذا النطاق. |
| [ClearContents](./clearcontents/) | يمسح محتويات هذا النطاق. |
| [ClearFormats](./clearformats/) | يمسح تنسيقات هذا النطاق. |
| [ClearComments](./clearcomments/) | يمسح تعليقات هذا النطاق. |
| [ClearHyperlinks](./clearhyperlinks/) | يزيل الروابط التشعبية فقط. |
