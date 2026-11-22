---
title: "الفئة Cells"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Cells. تغلف مجموعة من الكائنات المتعلقة بالخلية مثل Cell Row ...إلخ"
type: docs
url: /ar/net/aspose.cells/cells/
---
## Cells class

تغلف مجموعة من الكائنات المتعلقة بالخلية، مثل [`Cell`](../cell/), [`Row`](../row/), ...إلخ.

```csharp
public class Cells : IDisposable, IEnumerable
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Columns](../../aspose.cells/cells/columns/) { get; } | يحصل على مجموعة كائنات [`Column`](../column/) التي تمثل الأعمدة الفردية في ورقة العمل هذه. |
| [Count](../../aspose.cells/cells/count/) { get; } | يحصل على العدد الإجمالي لكائنات Cell المُنشأة. |
| [CountLarge](../../aspose.cells/cells/countlarge/) { get; } | يحصل على العدد الإجمالي لكائنات Cell المُنشأة. |
| [FirstCell](../../aspose.cells/cells/firstcell/) { get; } | يحصل على الخلية الأولى في ورقة العمل هذه. |
| [IsDefaultColumnHidden](../../aspose.cells/cells/isdefaultcolumnhidden/) { get; set; } |  |
| [IsDefaultRowHeightMatched](../../aspose.cells/cells/isdefaultrowheightmatched/) { get; set; } | يشير إلى أن ارتفاع الصف وارتفاع الخط الافتراضي متطابقان |
| [IsDefaultRowHidden](../../aspose.cells/cells/isdefaultrowhidden/) { get; set; } | يشير إلى ما إذا كان الصف مخفيًا بشكل افتراضي. |
| [Item](../../aspose.cells/cells/item/) { get; } | يحصل على عنصر [`Cell`](../cell/) في فهرس صف الخلية والعمود المحددين. (مؤشرين) |
| [LastCell](../../aspose.cells/cells/lastcell/) { get; } | يحصل على الخلية الأخيرة في ورقة العمل هذه. |
| [MaxColumn](../../aspose.cells/cells/maxcolumn/) { get; } | الحد الأقصى لفهرس العمود لتلك الخلايا التي تم إنشاؤها في المجموعة (لا تشمل العمود الذي تم تعريف النمط له للعمود بأكمله ولكن لم يتم إنشاء أي خلية فيه). |
| [MaxDataColumn](../../aspose.cells/cells/maxdatacolumn/) { get; } | الحد الأقصى لفهرس العمود للخلية التي تحتوي على بيانات. |
| [MaxDataRow](../../aspose.cells/cells/maxdatarow/) { get; } | الحد الأقصى لفهرس الصف للخلية التي تحتوي على بيانات. |
| [MaxDisplayRange](../../aspose.cells/cells/maxdisplayrange/) { get; } | يحصل على النطاق الأقصى الذي يشمل البيانات والخلايا المدمجة والأشكال. |
| [MaxRow](../../aspose.cells/cells/maxrow/) { get; } | الحد الأقصى لفهرس الصف للخلية التي تحتوي على بيانات أو نمط. |
| [MemorySetting](../../aspose.cells/cells/memorysetting/) { get; set; } | يحصل على أو يضبط خيار استخدام الذاكرة لهذه الخلايا. |
| [MergedCells](../../aspose.cells/cells/mergedcells/) { get; } | (**Obsolete.**) يحصل على مجموعة الخلايا المدمجة. |
| [MinColumn](../../aspose.cells/cells/mincolumn/) { get; } | الحد الأدنى لفهرس العمود لتلك الخلايا التي تم إنشاؤها في المجموعة (لا تشمل العمود الذي تم تعريف النمط له للعمود بأكمله ولكن لم يتم إنشاء أي خلية فيه). |
| [MinDataColumn](../../aspose.cells/cells/mindatacolumn/) { get; } | الحد الأدنى لفهرس العمود للخلية التي تحتوي على بيانات. |
| [MinDataRow](../../aspose.cells/cells/mindatarow/) { get; } | الحد الأدنى لمؤشر الصف للخلية التي تحتوي على بيانات. |
| [MinRow](../../aspose.cells/cells/minrow/) { get; } | الحد الأدنى لمؤشر الصف للخلية التي تحتوي على بيانات أو نمط. |
| [MultiThreadReading](../../aspose.cells/cells/multithreadreading/) { get; set; } | يحصل أو يعيّن ما إذا كان نموذج بيانات الخلايا يجب أن يدعم القراءة متعددة الخيوط. القيمة الافتراضية لهذه الخاصية هي false. |
| [OdsCellFields](../../aspose.cells/cells/odscellfields/) { get; } | يحصل على قائمة الحقول في ods. |
| [PreserveString](../../aspose.cells/cells/preservestring/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كانت جميع قيم ورقة العمل محفوظة كسلاسل. القيمة الافتراضية هي false. |
| [Ranges](../../aspose.cells/cells/ranges/) { get; } | يحصل على مجموعة كائنات [`Range`](../range/) التي تم إنشاؤها أثناء التشغيل. |
| [Rows](../../aspose.cells/cells/rows/) { get; } | يحصل على مجموعة كائنات [`Row`](../row/) التي تمثل الصفوف الفردية في ورقة العمل هذه. |
| [StandardHeight](../../aspose.cells/cells/standardheight/) { get; set; } | يحصل أو يعيّن ارتفاع الصف الافتراضي في ورقة العمل هذه، بوحدة النقاط. |
| [StandardHeightInch](../../aspose.cells/cells/standardheightinch/) { get; set; } | يحصل أو يعيّن ارتفاع الصف الافتراضي في ورقة العمل هذه، بوحدة البوصة. |
| [StandardHeightPixels](../../aspose.cells/cells/standardheightpixels/) { get; set; } | يحصل أو يعيّن ارتفاع الصف الافتراضي في ورقة العمل هذه، بوحدة البكسل. |
| [StandardWidth](../../aspose.cells/cells/standardwidth/) { get; set; } | يحصل أو يعيّن عرض العمود الافتراضي في ورقة العمل، بوحدة الأحرف. |
| [StandardWidthInch](../../aspose.cells/cells/standardwidthinch/) { get; set; } | يحصل أو يعيّن عرض العمود الافتراضي في ورقة العمل، بوحدة البوصة. |
| [StandardWidthPixels](../../aspose.cells/cells/standardwidthpixels/) { get; set; } | يحصل أو يعيّن عرض العمود الافتراضي في ورقة العمل، بوحدة البكسل. |
| [Style](../../aspose.cells/cells/style/) { get; set; } | يحصل ويعيّن النمط الافتراضي لورقة العمل. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [AddRange](../../aspose.cells/cells/addrange/)(Range) | يضيف مرجع كائن نطاق إلى الخلايا |
| [ApplyColumnStyle](../../aspose.cells/cells/applycolumnstyle/)(int, Style, StyleFlag) | يطبق التنسيقات على عمود كامل. |
| [ApplyRowStyle](../../aspose.cells/cells/applyrowstyle/)(int, Style, StyleFlag) | يطبق التنسيقات على الصف بأكمله. |
| [ApplyStyle](../../aspose.cells/cells/applystyle/)(Style, StyleFlag) | يطبق التنسيقات على ورقة عمل كاملة. |
| [CheckCell](../../aspose.cells/cells/checkcell/)(int, int) | يحصل على عنصر [`Cell`](../cell/) أو null عند مؤشر صف الخلية والعمود المحددين. |
| [CheckColumn](../../aspose.cells/cells/checkcolumn/)(int) | يحصل على عنصر [`Column`](../column/) أو null عند مؤشر العمود المحدد. |
| [CheckRow](../../aspose.cells/cells/checkrow/)(int) | يحصل على عنصر [`Row`](../row/) أو null عند مؤشر صف الخلية المحدد. |
| [Clear](../../aspose.cells/cells/clear/)() | يمسح جميع بيانات ورقة العمل. |
| [ClearContents](../../aspose.cells/cells/clearcontents/#clearcontents)(CellArea) | يمسح محتويات نطاق. |
| [ClearContents](../../aspose.cells/cells/clearcontents/#clearcontents_1)(int, int, int, int) | يمسح محتويات نطاق. |
| [ClearFormats](../../aspose.cells/cells/clearformats/#clearformats)(CellArea) | يمسح تنسيق نطاق. |
| [ClearFormats](../../aspose.cells/cells/clearformats/#clearformats_1)(int, int, int, int) | يمسح تنسيق نطاق. |
| [ClearMergedCells](../../aspose.cells/cells/clearmergedcells/)() | يمسح جميع النطاقات المدمجة. |
| [ClearRange](../../aspose.cells/cells/clearrange/#clearrange)(CellArea) | يمسح محتويات وتنسيق نطاق. |
| [ClearRange](../../aspose.cells/cells/clearrange/#clearrange_1)(int, int, int, int) | يمسح محتويات وتنسيق نطاق. |
| [ConvertStringToNumericValue](../../aspose.cells/cells/convertstringtonumericvalue/)() | يحوِّل جميع بيانات السلسلة في ورقة العمل إلى قيمة رقمية إذا أمكن. |
| [CopyColumn](../../aspose.cells/cells/copycolumn/)(Cells, int, int) | ينسخ البيانات والتنسيقات لعمود كامل. |
| [CopyColumns](../../aspose.cells/cells/copycolumns/#copycolumns)(Cells, int, int, int) | ينسخ البيانات والتنسيقات لأعمدة كاملة. |
| [CopyColumns](../../aspose.cells/cells/copycolumns/#copycolumns_2)(Cells, int, int, int, int) | ينسخ البيانات والتنسيقات للأعمدة الكاملة. |
| [CopyColumns](../../aspose.cells/cells/copycolumns/#copycolumns_1)(Cells, int, int, int, PasteOptions) | ينسخ البيانات والتنسيقات لعمود كامل. |
| [CopyRow](../../aspose.cells/cells/copyrow/)(Cells, int, int) | ينسخ البيانات والتنسيقات لصف كامل. |
| [CopyRows](../../aspose.cells/cells/copyrows/#copyrows)(Cells, int, int, int) | ينسخ البيانات والتنسيقات لبعض الصفوف الكاملة. |
| [CopyRows](../../aspose.cells/cells/copyrows/#copyrows_1)(Cells, int, int, int, CopyOptions) | ينسخ البيانات والتنسيقات لبعض الصفوف الكاملة. |
| [CopyRows](../../aspose.cells/cells/copyrows/#copyrows_2)(Cells, int, int, int, CopyOptions, PasteOptions) | ينسخ البيانات والتنسيقات لبعض الصفوف الكاملة. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange_2)(string) | ينشئ كائن [`Range`](../range/) من عنوان النطاق. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange_3)(string, string) | ينشئ كائن [`Range`](../range/) من نطاق من الخلايا. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange)(int, int, bool) | ينشئ كائن [`Range`](../range/) من صفوف الخلايا أو أعمدة الخلايا. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange_1)(int, int, int, int) | ينشئ كائن [`Range`](../range/) من نطاق من الخلايا. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns/#deleteblankcolumns)() | احذف جميع الأعمدة الفارغة التي لا تحتوي على أي بيانات. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns/#deleteblankcolumns_1)(DeleteOptions) | احذف جميع الأعمدة الفارغة التي لا تحتوي على أي بيانات. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows/#deleteblankrows)() | احذف جميع الصفوف الفارغة التي لا تحتوي على أي بيانات أو كائن آخر. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows/#deleteblankrows_1)(DeleteOptions) | احذف جميع الصفوف الفارغة التي لا تحتوي على أي بيانات أو بعض الكائنات الخاصة مثل التعليق المرئي، جدول محوري. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn/#deletecolumn)(int) | يحذف عمودًا. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn/#deletecolumn_1)(int, bool) | يحذف عمودًا. |
| [DeleteColumns](../../aspose.cells/cells/deletecolumns/#deletecolumns_1)(int, int, bool) | يحذف عدة أعمدة. |
| [DeleteColumns](../../aspose.cells/cells/deletecolumns/#deletecolumns)(int, int, DeleteOptions) | يحذف عدة أعمدة. |
| [DeleteRange](../../aspose.cells/cells/deleterange/)(int, int, int, int, ShiftType) | يحذف نطاقًا من الخلايا ويُحَرِّك الخلايا وفقًا لخيار الإزاحة. |
| [DeleteRow](../../aspose.cells/cells/deleterow/#deleterow)(int) | يحذف صفًا. |
| [DeleteRow](../../aspose.cells/cells/deleterow/#deleterow_1)(int, bool) | يحذف صفًا. |
| [DeleteRows](../../aspose.cells/cells/deleterows/#deleterows)(int, int) | يحذف عدة صفوف. |
| [DeleteRows](../../aspose.cells/cells/deleterows/#deleterows_2)(int, int, bool) | يحذف عدة صفوف في ورقة العمل. |
| [DeleteRows](../../aspose.cells/cells/deleterows/#deleterows_1)(int, int, DeleteOptions) | يحذف عدة صفوف في ورقة العمل. |
| [Dispose](../../aspose.cells/cells/dispose/)() | ينفّذ مهامًا معرفة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة تعيين الموارد غير المُدارة. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn/#endcellincolumn)(int) | يحصل على الخلية الأخيرة في هذا العمود. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn/#endcellincolumn_1)(int, int, int, int) | يحصل على الخلية الأخيرة ذات أعلى فهرس عمود في هذا النطاق. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow/#endcellinrow)(int) | يحصل على الخلية الأخيرة في هذا الصف. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow/#endcellinrow_1)(int, int, int, int) | يحصل على الخلية الأخيرة ذات أعلى فهرس صف في هذا النطاق. |
| [ExportArray](../../aspose.cells/cells/exportarray/)(int, int, int, int) | يصدّر البيانات في مجموعة `Cells` إلى كائن مصفوفة ثنائية الأبعاد. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable/#exportdatatable)(int, int, int, int) | يصدّر البيانات في مجموعة `Cells` إلى كائن DataTable. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable/#exportdatatable_2)(int, int, int, int, bool) | يصدّر البيانات في مجموعة `Cells` إلى كائن DataTable. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable/#exportdatatable_1)(int, int, int, int, ExportTableOptions) | يصدّر البيانات في مجموعة `Cells` إلى كائن DataTable. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring/#exportdatatableasstring)(int, int, int, int) | يصدّر البيانات في مجموعة `Cells` إلى كائن DataTable. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring/#exportdatatableasstring_1)(int, int, int, int, bool) | يصدّر البيانات في مجموعة `Cells` إلى كائن DataTable. |
| [ExportList&lt;T&gt;](../../aspose.cells/cells/exportlist/)(int, int, int, int, ExportTableOptions) |  |
| [ExportTypeArray](../../aspose.cells/cells/exporttypearray/)(int, int, int, int) | يصدّر نوع قيمة الخلية في مجموعة `Cells` إلى كائن مصفوفة ثنائية الأبعاد. |
| [Find](../../aspose.cells/cells/find/#find)(object, Cell) | يبحث عن الخلية التي تحتوي على الكائن المدخل. |
| [Find](../../aspose.cells/cells/find/#find_1)(object, Cell, FindOptions) | يبحث عن الخلية التي تحتوي على الكائن المدخل. |
| [GetCell](../../aspose.cells/cells/getcell/)(int, int) | (**Obsolete.**) يحصل على عنصر [`Cell`](../cell/) أو null في فهرس صف الخلية المحدد وفهرس عمود الخلية. |
| [GetCellDisplayStyle](../../aspose.cells/cells/getcelldisplaystyle/#getcelldisplaystyle)(int, int) | احصل على نمط العرض للخلية المعطاة. |
| [GetCellDisplayStyle](../../aspose.cells/cells/getcelldisplaystyle/#getcelldisplaystyle_1)(int, int, BorderType) | احصل على نمط العرض للخلية المعطاة. |
| [GetCellStyle](../../aspose.cells/cells/getcellstyle/)(int, int) | احصل على نمط الخلية المعطاة. |
| [GetCellsWithPlaceInCellPicture](../../aspose.cells/cells/getcellswithplaceincellpicture/)() | يحصل على جميع الخلايا التي تحتوي على صورة مدمجة. |
| [GetColumnOriginalWidthPoint](../../aspose.cells/cells/getcolumnoriginalwidthpoint/)(int) | (**Obsolete.**) يحصل على ارتفاع العمود الأصلي بوحدة النقطة إذا كان العمود مخفيًا. |
| [GetColumnWidth](../../aspose.cells/cells/getcolumnwidth/#getcolumnwidth)(int) | يحصل على عرض (بوحدة الأحرف) للعمود المحدد في العرض العادي. |
| [GetColumnWidth](../../aspose.cells/cells/getcolumnwidth/#getcolumnwidth_1)(int, bool, CellsUnitType) | يحصل على عرض العمود. |
| [GetColumnWidthInch](../../aspose.cells/cells/getcolumnwidthinch/)(int) | (**Obsolete.**) يحصل على عرض العمود المحدد في العرض العادي، بوحدة البوصة. |
| [GetColumnWidthPixel](../../aspose.cells/cells/getcolumnwidthpixel/#getcolumnwidthpixel)(int) | يحصل على عرض العمود المحدد في العرض العادي، بوحدة البكسل. |
| [GetColumnWidthPixel](../../aspose.cells/cells/getcolumnwidthpixel/#getcolumnwidthpixel_1)(int, bool) | (**Obsolete.**) يحصل على عرض العمود المحدد في العرض العادي، بوحدة البكسل. |
| [GetDependents](../../aspose.cells/cells/getdependents/)(bool, int, int) | احصل على جميع الخلايا التي تشير إلى الخلية المحددة. |
| [GetDependentsInCalculation](../../aspose.cells/cells/getdependentsincalculation/)(int, int, bool) | يحصل على جميع الخلايا التي تعتمد نتيجتها المحسوبة على الخلية المحددة. |
| [GetEnumerator](../../aspose.cells/cells/getenumerator/)() | يحصل على عداد الخلايا. |
| [GetFirstDataRow](../../aspose.cells/cells/getfirstdatarow/)(int) | يحصل على فهرس الصف الأول للخلية التي تحتوي على بيانات في العمود المحدد. |
| [GetGroupedColumnOutlineLevel](../../aspose.cells/cells/getgroupedcolumnoutlinelevel/)(int) | يحصل على مستوى المخطط (بدءًا من الصفر) للعمود. |
| [GetGroupedRowOutlineLevel](../../aspose.cells/cells/getgroupedrowoutlinelevel/)(int) | يحصل على مستوى المخطط (بدءًا من الصفر) للصف. |
| [GetLastDataRow](../../aspose.cells/cells/getlastdatarow/)(int) | يحصل على فهرس الصف الأخير للخلية التي تحتوي على بيانات في العمود المحدد. |
| [GetMaxGroupedColumnOutlineLevel](../../aspose.cells/cells/getmaxgroupedcolumnoutlinelevel/)() | يحصل على الحد الأقصى لمستوى مخطط العمود المجمّع (بدءًا من الصفر). |
| [GetMaxGroupedRowOutlineLevel](../../aspose.cells/cells/getmaxgroupedrowoutlinelevel/)() | يحصل على الحد الأقصى لمستوى مخطط الصف المجمّع (بدءًا من الصفر). |
| [GetMergedAreas](../../aspose.cells/cells/getmergedareas/)() | يحصل على جميع الخلايا المدمجة. |
| [GetRow](../../aspose.cells/cells/getrow/)(int) | (**Obsolete.**) يحصل على عنصر [`Row`](../row/) في فهرس صف الخلية المحدد. |
| [GetRowEnumerator](../../aspose.cells/cells/getrowenumerator/)() | (**Obsolete.**) يحصل على عداد الصفوف. |
| [GetRowHeight](../../aspose.cells/cells/getrowheight/#getrowheight)(int) | يحصل على ارتفاع صف محدد، بوحدة النقاط. |
| [GetRowHeight](../../aspose.cells/cells/getrowheight/#getrowheight_1)(int, bool, CellsUnitType) | يحصل على ارتفاع الصف. |
| [GetRowHeightInch](../../aspose.cells/cells/getrowheightinch/)(int) | يحصل على ارتفاع صف محدد بوحدة البوصة. |
| [GetRowHeightPixel](../../aspose.cells/cells/getrowheightpixel/)(int) | يحصل على ارتفاع الصف المحدد بوحدة البكسل. |
| [GetRowOriginalHeightPoint](../../aspose.cells/cells/getroworiginalheightpoint/)(int) | (**Obsolete.**) يحصل على ارتفاع الصف الأصلي بوحدة النقطة إذا كان الصف مخفيًا |
| [GetViewColumnWidthPixel](../../aspose.cells/cells/getviewcolumnwidthpixel/)(int) | احصل على العرض في نوع عرض مختلف. |
| [GetViewRowHeight](../../aspose.cells/cells/getviewrowheight/)(int) | يحصل على ارتفاع الصف المحدد. |
| [GetViewRowHeightInch](../../aspose.cells/cells/getviewrowheightinch/)(int) | يحصل على ارتفاع صف محدد بوحدة البوصة. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns/#groupcolumns)(int, int) | يقوم بتجميع الأعمدة. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns/#groupcolumns_1)(int, int, bool) | يقوم بتجميع الأعمدة. |
| [GroupRows](../../aspose.cells/cells/grouprows/#grouprows)(int, int) | يقوم بتجميع الصفوف. |
| [GroupRows](../../aspose.cells/cells/grouprows/#grouprows_1)(int, int, bool) | يقوم بتجميع الصفوف. |
| [HideColumn](../../aspose.cells/cells/hidecolumn/)(int) | يخفي عمودًا. |
| [HideColumns](../../aspose.cells/cells/hidecolumns/)(int, int) | إخفاء أعمدة متعددة. |
| [HideGroupDetail](../../aspose.cells/cells/hidegroupdetail/)(bool, int) | يطوي الصفوف/الأعمدة المجمعة. |
| [HideRow](../../aspose.cells/cells/hiderow/)(int) | يخفي صفًا. |
| [HideRows](../../aspose.cells/cells/hiderows/)(int, int) | يخفي صفوفًا متعددة. |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray)(double[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_2)(int[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_4)(string[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_1)(double[], int, int, bool) | يستورد مصفوفة من double إلى ورقة عمل. |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_3)(int[], int, int, bool) | يستورد مصفوفة من integer إلى ورقة عمل. |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_5)(string[], int, int, bool) | يستورد مصفوفة من string إلى ورقة عمل. |
| [ImportArrayList](../../aspose.cells/cells/importarraylist/)(ArrayList, int, int, bool) | يستورد arraylist من البيانات إلى ورقة عمل. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv)(Stream, TxtLoadOptions, int, int) | استيراد ملف CSV إلى الخلايا. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv_2)(string, TxtLoadOptions, int, int) | استيراد ملف CSV إلى الخلايا. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv_1)(Stream, string, bool, int, int) | استيراد ملف CSV إلى الخلايا. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv_3)(string, string, bool, int, int) | استيراد ملف CSV إلى الخلايا. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects/#importcustomobjects)(ICollection, int, int, ImportTableOptions) | يستورد كائنات مخصصة. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects/#importcustomobjects_1)(ICollection, string[], bool, int, int, int, bool, string, bool) | يستورد كائنات مخصصة. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_3)(IDataReader, int, int) | يستورد البيانات من كائن IDataReader. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_1)(DataTable, int, int, ImportTableOptions) | استيراد البيانات من جدول بيانات مخصص. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_2)(DataView, int, int, ImportTableOptions) | استيراد البيانات من DataView. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata)(ICellsDataTable, int, int, ImportTableOptions) | استيراد البيانات من جدول بيانات مخصص. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_4)(IDataReader, int, int, ImportTableOptions) | يستورد البيانات من كائن IDataReader. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid/#importdatagrid)(DataGrid, int, int, bool) | يستورد DataGrid إلى ورقة عمل. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid/#importdatagrid_1)(DataGrid, int, int, int, int, bool) | يستورد DataGrid إلى ورقة عمل. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid/#importdatagrid_2)(DataGrid, int, int, int, int, bool, bool) | يستورد DataGrid إلى ورقة عمل. |
| [ImportDataGridAsString](../../aspose.cells/cells/importdatagridasstring/)(DataGrid, int, int, bool) | يستورد DataGrid إلى ورقة عمل. لا تحاول هذه الطريقة تحويل النص إلى قيم رقمية. |
| [ImportDataRow](../../aspose.cells/cells/importdatarow/)(DataRow, int, int) | يستورد DataRow إلى ملف Excel. |
| [ImportDataView](../../aspose.cells/cells/importdataview/)(DataView, int, int) | يستورد DataView إلى ورقة عمل. |
| [ImportFormulaArray](../../aspose.cells/cells/importformulaarray/)(string[], int, int, bool) | يستورد مصفوفة من الصيغ إلى ورقة عمل. |
| [ImportGridView](../../aspose.cells/cells/importgridview/)(GridView, int, int, ImportTableOptions) | يستورد عرض شبكة إلى هذه الخلايا. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray/#importobjectarray)(object[], int, int, bool) | يستورد مصفوفة من البيانات إلى ورقة عمل. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray/#importobjectarray_1)(object[], int, int, bool, int) | يستورد مصفوفة من البيانات إلى ورقة عمل. |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray)(object[], int, int) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray_1)(object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray_3)(object[], object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray_2)(object[], object[], int, int, TxtLoadOptions) |  |
| [InsertColumn](../../aspose.cells/cells/insertcolumn/#insertcolumn)(int) | يدرج عمودًا جديدًا في ورقة العمل. |
| [InsertColumn](../../aspose.cells/cells/insertcolumn/#insertcolumn_1)(int, bool) | يدرج عمودًا جديدًا في ورقة العمل. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns/#insertcolumns)(int, int) | يدرج بعض الأعمدة في ورقة العمل. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns/#insertcolumns_2)(int, int, bool) | يدرج بعض الأعمدة في ورقة العمل. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns/#insertcolumns_1)(int, int, InsertOptions) | يدرج بعض الأعمدة في ورقة العمل. |
| [InsertCutCells](../../aspose.cells/cells/insertcutcells/)(Range, int, int, ShiftType) | إدراج نطاق مقطوع. |
| [InsertRange](../../aspose.cells/cells/insertrange/#insertrange)(CellArea, ShiftType) | يدرج نطاقًا من الخلايا ويُحرك الخلايا وفقًا لخيار التحريك. |
| [InsertRange](../../aspose.cells/cells/insertrange/#insertrange_1)(CellArea, int, ShiftType) | يدرج نطاقًا من الخلايا ويُحرك الخلايا وفقًا لخيار التحريك. |
| [InsertRange](../../aspose.cells/cells/insertrange/#insertrange_2)(CellArea, int, ShiftType, bool) | يدرج نطاقًا من الخلايا ويُحرك الخلايا وفقًا لخيار التحريك. |
| [InsertRow](../../aspose.cells/cells/insertrow/)(int) | يدرج صفًا جديدًا في ورقة العمل. |
| [InsertRows](../../aspose.cells/cells/insertrows/#insertrows)(int, int) | يدرج عدة صفوف في ورقة العمل. |
| [InsertRows](../../aspose.cells/cells/insertrows/#insertrows_2)(int, int, bool) | يدرج عدة صفوف في ورقة العمل. |
| [InsertRows](../../aspose.cells/cells/insertrows/#insertrows_1)(int, int, InsertOptions) | يدرج عدة صفوف في ورقة العمل. |
| [IsBlankColumn](../../aspose.cells/cells/isblankcolumn/)(int) | يتحقق مما إذا كان العمود المحدد فارغًا (لا يحتوي على أي بيانات). |
| [IsColumnHidden](../../aspose.cells/cells/iscolumnhidden/)(int) | يتحقق مما إذا كان العمود في الفهرس المحدد مخفيًا. |
| [IsDeletingRangeEnabled](../../aspose.cells/cells/isdeletingrangeenabled/)(int, int, int, int) | تحقق مما إذا كان يمكن حذف النطاق. |
| [IsRowHidden](../../aspose.cells/cells/isrowhidden/)(int) | يتحقق مما إذا كان الصف في الفهرس المحدد مخفيًا. |
| [LinkToXmlMap](../../aspose.cells/cells/linktoxmlmap/)(string, int, int, string) | رابط إلى خريطة XML. |
| [Merge](../../aspose.cells/cells/merge/#merge)(int, int, int, int) | يدمج نطاقًا محددًا من الخلايا في خلية واحدة. |
| [Merge](../../aspose.cells/cells/merge/#merge_1)(int, int, int, int, bool) | يدمج نطاقًا محددًا من الخلايا في خلية واحدة. |
| [Merge](../../aspose.cells/cells/merge/#merge_2)(int, int, int, int, bool, bool) | يدمج نطاقًا محددًا من الخلايا في خلية واحدة. |
| [MoveRange](../../aspose.cells/cells/moverange/)(CellArea, int, int) | ينقل النطاق. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates/#removeduplicates)() | يزيل الصفوف المكررة في الورقة. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates/#removeduplicates_1)(int, int, int, int) | يزيل القيم المكررة في النطاق. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates/#removeduplicates_2)(int, int, int, int, bool, int[]) | يزيل البيانات المكررة في النطاق. |
| [RemoveFormulas](../../aspose.cells/cells/removeformulas/)() | يزيل جميع الصيغ ويستبدلها بقيمة الصيغة. |
| [RetrieveSubtotalSetting](../../aspose.cells/cells/retrievesubtotalsetting/)(CellArea) | يسترجع إعدادات المجاميع الفرعية للنطاق. |
| [SetColumnWidth](../../aspose.cells/cells/setcolumnwidth/)(int, double) | يضبط عرض العمود المحدد في العرض العادي. |
| [SetColumnWidthInch](../../aspose.cells/cells/setcolumnwidthinch/)(int, double) | يضبط عرض العمود بوحدة البوصة في العرض العادي. |
| [SetColumnWidthPixel](../../aspose.cells/cells/setcolumnwidthpixel/)(int, int) | يضبط عرض العمود بوحدة البكسل في العرض العادي. |
| [SetRowHeight](../../aspose.cells/cells/setrowheight/)(int, double) | يضبط ارتفاع الصف المحدد. |
| [SetRowHeightInch](../../aspose.cells/cells/setrowheightinch/)(int, double) | يضبط ارتفاع الصف بوحدة البوصة. |
| [SetRowHeightPixel](../../aspose.cells/cells/setrowheightpixel/)(int, int) | يضبط ارتفاع الصف بوحدة البكسل. |
| [SetViewColumnWidthPixel](../../aspose.cells/cells/setviewcolumnwidthpixel/)(int, int) | يضبط عرض العمود في عرض مختلف. |
| [ShowGroupDetail](../../aspose.cells/cells/showgroupdetail/)(bool, int) | يوسع الصفوف/الأعمدة المجمعة. |
| [Subtotal](../../aspose.cells/cells/subtotal/#subtotal)(CellArea, int, ConsolidationFunction, int[]) | ينشئ المجاميع الفرعية للنطاق. |
| [Subtotal](../../aspose.cells/cells/subtotal/#subtotal_1)(CellArea, int, ConsolidationFunction, int[], bool, bool, bool) | ينشئ المجاميع الفرعية للنطاق. |
| [TextToColumns](../../aspose.cells/cells/texttocolumns/)(int, int, int, TxtLoadOptions) | يقسم المحتوى في العمود المحدد إلى عدة أعمدة.. |
| [UngroupColumns](../../aspose.cells/cells/ungroupcolumns/)(int, int) | يفك تجميع الأعمدة. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows/#ungrouprows)(int, int) | يفك تجميع الصفوف. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows/#ungrouprows_1)(int, int, bool) | يفك تجميع الصفوف. |
| [UnhideColumn](../../aspose.cells/cells/unhidecolumn/)(int, double) | يكشف عن عمود |
| [UnhideColumns](../../aspose.cells/cells/unhidecolumns/)(int, int, double) | يكشف عن عدة أعمدة. |
| [UnhideRow](../../aspose.cells/cells/unhiderow/)(int, double) | يكشف عن صف. |
| [UnhideRows](../../aspose.cells/cells/unhiderows/)(int, int, double) | يكشف عن الصفوف المخفية. |
| [UnMerge](../../aspose.cells/cells/unmerge/)(int, int, int, int) | يفك دمج نطاق محدد من الخلايا المدمجة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsDemo
    {
        public static void CellsExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تعيين ارتفاع الصف الافتراضي
            cells.StandardHeight = 20;
            // تعيين ارتفاع الصف
            cells.SetRowHeight(2, 20.5);

            // تعيين عرض العمود الافتراضي
            cells.StandardWidth = 15;
            // تعيين عرض العمود
            cells.SetColumnWidth(3, 12.57);

            // دمج الخلايا
            cells.Merge(5, 4, 2, 2);

            // إدخال القيم في الخلايا
            cells[0, 0].PutValue(true);
            cells[0, 1].PutValue(1);
            cells[0, 2].PutValue("abc");

            // تصدير البيانات
            object[,] arr = cells.ExportArray(0, 0, 10, 10);

            // عرض بعض الخصائص
            Console.WriteLine("Total Cells Count: " + cells.Count);
            Console.WriteLine("Total Cells Count (Large): " + cells.CountLarge);
            Console.WriteLine("Min Row with Data: " + cells.MinDataRow);
            Console.WriteLine("Max Row with Data: " + cells.MaxDataRow);
            Console.WriteLine("Min Column with Data: " + cells.MinDataColumn);
            Console.WriteLine("Max Column with Data: " + cells.MaxDataColumn);

            // التكرار عبر الخلايا
            IEnumerator enumerator = cells.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                Console.WriteLine(cell.Name + ": " + cell.Value);
            }

            // احفظ المصنف
            workbook.Save("CellsExample.xlsx");
            workbook.Save("CellsExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


