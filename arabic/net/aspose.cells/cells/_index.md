---
title: Cells
second_title: Aspose.Cells لمرجع .NET API
description: لتضمين مجموعة من الكائنات ذات الصلة بالخلايا  مثلCell./cell وRow./row ... الخ.
type: docs
weight: 300
url: /ar/net/aspose.cells/cells/
---
## Cells class

لتضمين مجموعة من الكائنات ذات الصلة بالخلايا ، مثل[`Cell`](../cell) و[`Row`](../row)، ... الخ.

```csharp
public class Cells : IDisposable, IEnumerable
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [Columns](../../aspose.cells/cells/columns) { get; } | يحصل على مجموعة[`Column`](../column) كائنات تمثل الأعمدة الفردية في ورقة العمل هذه. |
| [Count](../../aspose.cells/cells/count) { get; } | الحصول على العدد الإجمالي لكائنات الخلية التي تم إنشاء مثيل لها. |
| [CountLarge](../../aspose.cells/cells/countlarge) { get; } | الحصول على العدد الإجمالي لكائنات الخلية التي تم إنشاء مثيل لها. |
| [FirstCell](../../aspose.cells/cells/firstcell) { get; } | يحصل على الخلية الأولى في ورقة العمل هذه. |
| [IsDefaultRowHeightMatched](../../aspose.cells/cells/isdefaultrowheightmatched) { get; set; } | يشير إلى أن ارتفاع الصف وارتفاع الخط الافتراضي يتطابقان مع |
| [IsDefaultRowHidden](../../aspose.cells/cells/isdefaultrowhidden) { get; set; } | يشير إلى ما إذا كان الصف مخفيًا افتراضيًا. |
| [Item](../../aspose.cells/cells/item) { get; } | يحصل على ملف[`Cell`](../cell) عنصر في فهرس صف الخلية المحدد وفهرس العمود. (2 indexers) |
| [LastCell](../../aspose.cells/cells/lastcell) { get; } | الحصول على الخلية الأخيرة في ورقة العمل هذه. |
| [MaxColumn](../../aspose.cells/cells/maxcolumn) { get; } | الحد الأدنى لفهرس العمود لتلك الخلايا التي تم تكوين مثيل لها في المجموعة (لا يتضمن العمود حيث يتم تعريف النمط للعمود بأكمله ولكن لم يتم إنشاء مثيل لأي خلية فيه) . |
| [MaxDataColumn](../../aspose.cells/cells/maxdatacolumn) { get; } | الحد الأقصى لفهرس العمود للخلية التي تحتوي على بيانات . |
| [MaxDataRow](../../aspose.cells/cells/maxdatarow) { get; } | الحد الأقصى لفهرس صف الخلية الذي يحتوي على بيانات . |
| [MaxDisplayRange](../../aspose.cells/cells/maxdisplayrange) { get; } | الحصول على النطاق الأقصى الذي يتضمن البيانات والخلايا والأشكال المدمجة. |
| [MaxRow](../../aspose.cells/cells/maxrow) { get; } | الحد الأقصى لفهرس صف الخلية الذي يحتوي على بيانات أو نمط . |
| [MemorySetting](../../aspose.cells/cells/memorysetting) { get; set; } | الحصول على أو تعيين خيار استخدام الذاكرة لهذه الخلايا. |
| [MergedCells](../../aspose.cells/cells/mergedcells) { get; } | الحصول على مجموعة الخلايا المدمجة. |
| [MinColumn](../../aspose.cells/cells/mincolumn) { get; } | الحد الأدنى لفهرس العمود لتلك الخلايا التي تم تكوين مثيل لها في المجموعة (لا يتضمن العمود حيث يتم تعريف النمط للعمود بأكمله ولكن لم يتم إنشاء مثيل لأي خلية فيه) . |
| [MinDataColumn](../../aspose.cells/cells/mindatacolumn) { get; } | الحد الأدنى لفهرس العمود للخلية الذي يحتوي على بيانات . |
| [MinDataRow](../../aspose.cells/cells/mindatarow) { get; } | الحد الأدنى لفهرس صف الخلية الذي يحتوي على بيانات. |
| [MinRow](../../aspose.cells/cells/minrow) { get; } | الحد الأدنى لفهرس صف الخلية الذي يحتوي على بيانات أو نمط . |
| [MultiThreadReading](../../aspose.cells/cells/multithreadreading) { get; set; } | الحصول على أو تحديد ما إذا كان يجب أن يدعم نموذج بيانات الخلايا القراءة متعددة الخيوط . القيمة الافتراضية لهذه الخاصية خاطئة. |
| [OdsCellFields](../../aspose.cells/cells/odscellfields) { get; } | يحصل على قائمة الحقول ods. |
| [PreserveString](../../aspose.cells/cells/preservestring) { get; set; } | الحصول على قيمة أو تعيينها للإشارة إلى ما إذا كان سيتم الاحتفاظ بجميع قيم ورقة العمل كسلاسل أم لا. الافتراضي هو خطأ . |
| [Ranges](../../aspose.cells/cells/ranges) { get; } | يحصل على مجموعة[`Range`](../range)الكائنات التي تم إنشاؤها في وقت التشغيل. |
| [Rows](../../aspose.cells/cells/rows) { get; } | يحصل على مجموعة[`Row`](../row) كائنات تمثل الصفوف الفردية في ورقة العمل هذه. |
| [StandardHeight](../../aspose.cells/cells/standardheight) { get; set; } | الحصول على أو تعيين الارتفاع الافتراضي للصف في ورقة العمل هذه ، بوحدة النقاط. |
| [StandardHeightInch](../../aspose.cells/cells/standardheightinch) { get; set; } | الحصول على أو تعيين الارتفاع الافتراضي للصف في ورقة العمل هذه ، بوحدة البوصة. |
| [StandardHeightPixels](../../aspose.cells/cells/standardheightpixels) { get; set; } | الحصول على أو تعيين الارتفاع الافتراضي للصف في ورقة العمل هذه ، بوحدة البكسل. |
| [StandardWidth](../../aspose.cells/cells/standardwidth) { get; set; } | الحصول على أو تعيين عرض العمود الافتراضي في ورقة العمل ، في وحدة من الأحرف. |
| [StandardWidthInch](../../aspose.cells/cells/standardwidthinch) { get; set; } | الحصول على أو تعيين عرض العمود الافتراضي في ورقة العمل ، بوحدة البوصة. |
| [StandardWidthPixels](../../aspose.cells/cells/standardwidthpixels) { get; set; } | الحصول على أو تعيين عرض العمود الافتراضي في ورقة العمل ، بوحدة البكسل. |
| [Style](../../aspose.cells/cells/style) { get; set; } | الحصول على النمط الافتراضي وتعيينه. |

## طُرق

| اسم | وصف |
| --- | --- |
| [AddRange](../../aspose.cells/cells/addrange)(Range) | يضيف مرجع كائن النطاق إلى الخلايا |
| [ApplyColumnStyle](../../aspose.cells/cells/applycolumnstyle)(int, Style, StyleFlag) | يتم تطبيق تنسيقات لعمود كامل. |
| [ApplyRowStyle](../../aspose.cells/cells/applyrowstyle)(int, Style, StyleFlag) | يطبق التنسيقات على صف كامل . |
| [ApplyStyle](../../aspose.cells/cells/applystyle)(Style, StyleFlag) | يطبق التنسيقات على ورقة عمل كاملة . |
| [CheckCell](../../aspose.cells/cells/checkcell)(int, int) | يحصل على ملف[`Cell`](../cell) عنصر أو فارغ في فهرس صف الخلية المحدد وفهرس العمود. |
| [CheckColumn](../../aspose.cells/cells/checkcolumn)(int) | يحصل على ملف[`Column`](../column) عنصر أو فارغ في فهرس العمود المحدد. |
| [CheckRow](../../aspose.cells/cells/checkrow)(int) | يحصل على ملف[`Row`](../row) عنصر أو في فهرس صف الخلية المحدد. |
| [Clear](../../aspose.cells/cells/clear)() | مسح كافة كائنات الخلايا والصف . |
| [ClearContents](../../aspose.cells/cells/clearcontents#clearcontents)(CellArea) | يمسح محتويات النطاق . |
| [ClearContents](../../aspose.cells/cells/clearcontents#clearcontents_1)(int, int, int, int) | يمسح محتويات النطاق . |
| [ClearFormats](../../aspose.cells/cells/clearformats#clearformats)(CellArea) | مسح تنسيق النطاق. |
| [ClearFormats](../../aspose.cells/cells/clearformats#clearformats_1)(int, int, int, int) | مسح تنسيق النطاق. |
| [ClearMergedCells](../../aspose.cells/cells/clearmergedcells)() | مسح كافة النطاقات المدمجة. |
| [ClearRange](../../aspose.cells/cells/clearrange#clearrange)(CellArea) | يمسح محتويات وتنسيق النطاق. |
| [ClearRange](../../aspose.cells/cells/clearrange#clearrange_1)(int, int, int, int) | يمسح محتويات وتنسيق النطاق. |
| [ConvertStringToNumericValue](../../aspose.cells/cells/convertstringtonumericvalue)() | تحويل بيانات السلسلة في الخلايا إلى قيمة رقمية إن أمكن. |
| [CopyColumn](../../aspose.cells/cells/copycolumn)(Cells, int, int) | نسخ البيانات والتنسيقات لعمود كامل. |
| [CopyColumns](../../aspose.cells/cells/copycolumns#copycolumns)(Cells, int, int, int) | نسخ البيانات والتنسيقات لعمود كامل. |
| [CopyColumns](../../aspose.cells/cells/copycolumns#copycolumns_2)(Cells, int, int, int, int) | نسخ البيانات وتنسيقات الأعمدة بأكملها. |
| [CopyColumns](../../aspose.cells/cells/copycolumns#copycolumns_1)(Cells, int, int, int, PasteOptions) | نسخ البيانات والتنسيقات لعمود كامل. |
| [CopyRow](../../aspose.cells/cells/copyrow)(Cells, int, int) | نسخ بيانات وتنسيقات صف كامل. |
| [CopyRows](../../aspose.cells/cells/copyrows#copyrows)(Cells, int, int, int) | نسخ بيانات وتنسيقات لبعض الصفوف بأكملها. |
| [CopyRows](../../aspose.cells/cells/copyrows#copyrows_1)(Cells, int, int, int, CopyOptions) | نسخ بيانات وتنسيقات لبعض الصفوف بأكملها. |
| [CopyRows](../../aspose.cells/cells/copyrows#copyrows_2)(Cells, int, int, int, CopyOptions, PasteOptions) | نسخ بيانات وتنسيقات لبعض الصفوف بأكملها. |
| [CreateRange](../../aspose.cells/cells/createrange#createrange_2)(string) | ينشئ ملف[`Range`](../range) كائن من عنوان النطاق . |
| [CreateRange](../../aspose.cells/cells/createrange#createrange_3)(string, string) | ينشئ ملف[`Range`](../range) كائن من نطاق من الخلايا . |
| [CreateRange](../../aspose.cells/cells/createrange#createrange)(int, int, bool) | ينشئ ملف[`Range`](../range) كائن من صفوف الخلايا أو أعمدة الخلايا . |
| [CreateRange](../../aspose.cells/cells/createrange#createrange_1)(int, int, int, int) | ينشئ ملف[`Range`](../range) كائن من نطاق من الخلايا . |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns#deleteblankcolumns)() | احذف جميع الأعمدة الفارغة التي لا تحتوي على أي بيانات. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns#deleteblankcolumns_1)(DeleteOptions) | احذف جميع الأعمدة الفارغة التي لا تحتوي على أي بيانات. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows#deleteblankrows)() | احذف جميع الصفوف الفارغة التي لا تحتوي على أي بيانات. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows#deleteblankrows_1)(DeleteOptions) | احذف جميع الصفوف الفارغة التي لا تحتوي على أي بيانات. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn#deletecolumn)(int) | حذف عمود . |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn#deletecolumn_1)(int, bool) | حذف عمود . |
| [DeleteColumns](../../aspose.cells/cells/deletecolumns)(int, int, bool) | حذف عدة أعمدة . |
| [DeleteRange](../../aspose.cells/cells/deleterange)(int, int, int, int, ShiftType) | حذف نطاق من الخلايا وإزاحة الخلايا وفقًا لخيار الإزاحة. |
| [DeleteRow](../../aspose.cells/cells/deleterow)(int) | حذف صف . |
| [DeleteRows](../../aspose.cells/cells/deleterows#deleterows)(int, int) | حذف عدة صفوف . |
| [DeleteRows](../../aspose.cells/cells/deleterows#deleterows_1)(int, int, bool) | حذف عدة صفوف من ورقة العمل . |
| [Dispose](../../aspose.cells/cells/dispose)() | يؤدي مهام محددة بواسطة التطبيق مرتبطة بتحرير الموارد غير المُدارة أو تحريرها أو إعادة تعيينها. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn#endcellincolumn)(short) | الحصول على الخلية الأخيرة في هذا العمود . |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn#endcellincolumn_1)(int, int, short, short) | الحصول على الخلية الأخيرة ذات فهرس العمود الأقصى في هذا النطاق. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow#endcellinrow)(int) | الحصول على الخلية الأخيرة في هذا الصف . |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow#endcellinrow_1)(int, int, int, int) | الحصول على الخلية الأخيرة ذات فهرس الصف الأقصى في هذا النطاق. |
| [ExportArray](../../aspose.cells/cells/exportarray)(int, int, int, int) | يتم تصدير البيانات بتنسيق[`Cells`](../cells) المجموعة إلى كائن مصفوفة ثنائية الأبعاد. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable#exportdatatable)(int, int, int, int) | يتم تصدير البيانات بتنسيق[`Cells`](../cells) جمع لDataTable الكائن . |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable#exportdatatable_2)(int, int, int, int, bool) | يتم تصدير البيانات بتنسيق[`Cells`](../cells) جمع لDataTable الكائن . |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable#exportdatatable_1)(int, int, int, int, ExportTableOptions) | يتم تصدير البيانات بتنسيق[`Cells`](../cells) جمع لDataTable الكائن . |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring#exportdatatableasstring)(int, int, int, int) | يتم تصدير البيانات بتنسيق[`Cells`](../cells) جمع لDataTable الكائن . |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring#exportdatatableasstring_1)(int, int, int, int, bool) | يتم تصدير البيانات بتنسيق[`Cells`](../cells) جمع لDataTable الكائن . |
| [ExportTypeArray](../../aspose.cells/cells/exporttypearray)(int, int, int, int) | يصدر نوع قيمة الخلية في ملف[`Cells`](../cells) المجموعة إلى كائن مصفوفة ثنائية الأبعاد. |
| [Find](../../aspose.cells/cells/find#find)(object, Cell) | البحث عن الخلية التي تحتوي على كائن الإدخال. |
| [Find](../../aspose.cells/cells/find#find_1)(object, Cell, FindOptions) | البحث عن الخلية التي تحتوي على كائن الإدخال. |
| [GetCell](../../aspose.cells/cells/getcell)(int, int) | يحصل على ملف[`Cell`](../cell) عنصر أو فارغ في فهرس صف الخلية المحدد وفهرس العمود. |
| [GetCellStyle](../../aspose.cells/cells/getcellstyle)(int, int) | احصل على نمط الخلية المحددة . |
| [GetColumnWidth](../../aspose.cells/cells/getcolumnwidth)(int) | الحصول على عرض العمود المحدد في العرض العادي |
| [GetColumnWidthInch](../../aspose.cells/cells/getcolumnwidthinch)(int) | الحصول على عرض العمود المحدد في العرض العادي ، بوحدات البوصة . |
| [GetColumnWidthPixel](../../aspose.cells/cells/getcolumnwidthpixel)(int) | الحصول على عرض العمود المحدد في العرض العادي ، بوحدات البكسل. |
| [GetDependents](../../aspose.cells/cells/getdependents)(bool, int, int) | احصل على جميع الخلايا التي تشير إلى الخلية المحددة. |
| [GetDependentsInCalculation](../../aspose.cells/cells/getdependentsincalculation)(int, int, bool) | يحصل على جميع الخلايا التي تعتمد نتيجتها المحسوبة على خلية معينة. |
| [GetEnumerator](../../aspose.cells/cells/getenumerator)() | الحصول على تعداد الخلايا . |
| [GetGroupedColumnOutlineLevel](../../aspose.cells/cells/getgroupedcolumnoutlinelevel)(int) | يحصل على مستوى المخطط التفصيلي (على أساس الصفر) للعمود. |
| [GetGroupedRowOutlineLevel](../../aspose.cells/cells/getgroupedrowoutlinelevel)(int) | يحصل على مستوى المخطط التفصيلي (على أساس الصفر) للصف . |
| [GetLastDataRow](../../aspose.cells/cells/getlastdatarow)(int) | الحصول على فهرس الصف الأخير للخلية الذي يحتوي على بيانات في العمود المحدد. |
| [GetMaxGroupedColumnOutlineLevel](../../aspose.cells/cells/getmaxgroupedcolumnoutlinelevel)() | الحصول على الحد الأقصى لمستوى المخطط التفصيلي للعمود المُجمَّع (مستند إلى الصفر) . |
| [GetMaxGroupedRowOutlineLevel](../../aspose.cells/cells/getmaxgroupedrowoutlinelevel)() | الحصول على الحد الأقصى لمستوى المخطط التفصيلي للصف المجمع (على أساس الصفر) . |
| [GetRow](../../aspose.cells/cells/getrow)(int) | يحصل على ملف[`Row`](../row) عنصر في فهرس صف الخلية المحدد. |
| [GetRowEnumerator](../../aspose.cells/cells/getrowenumerator)() | يحصل على تعداد الصفوف. |
| [GetRowHeight](../../aspose.cells/cells/getrowheight)(int) | الحصول على ارتفاع صف معين. |
| [GetRowHeightInch](../../aspose.cells/cells/getrowheightinch)(int) | الحصول على ارتفاع صف محدد بوحدة البوصة . |
| [GetRowHeightPixel](../../aspose.cells/cells/getrowheightpixel)(int) | الحصول على ارتفاع صف محدد بوحدة البكسل . |
| [GetRowOriginalHeightPoint](../../aspose.cells/cells/getroworiginalheightpoint)(int) | الحصول على ارتفاع الصف الأصلي بوحدة النقطة إذا كان الصف مخفيًا |
| [GetViewColumnWidthPixel](../../aspose.cells/cells/getviewcolumnwidthpixel)(int) | احصل على العرض بنوع عرض مختلف . |
| [GetViewRowHeight](../../aspose.cells/cells/getviewrowheight)(int) | الحصول على ارتفاع صف معين. |
| [GetViewRowHeightInch](../../aspose.cells/cells/getviewrowheightinch)(int) | الحصول على ارتفاع صف محدد بوحدة البوصة . |
| [GroupColumns](../../aspose.cells/cells/groupcolumns#groupcolumns)(int, int) | أعمدة المجموعات. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns#groupcolumns_1)(int, int, bool) | أعمدة المجموعات. |
| [GroupRows](../../aspose.cells/cells/grouprows#grouprows)(int, int) | صفوف المجموعات . |
| [GroupRows](../../aspose.cells/cells/grouprows#grouprows_1)(int, int, bool) | صفوف المجموعات . |
| [HideColumn](../../aspose.cells/cells/hidecolumn)(int) | إخفاء عمود . |
| [HideColumns](../../aspose.cells/cells/hidecolumns)(int, int) | إخفاء عدة أعمدة . |
| [HideGroupDetail](../../aspose.cells/cells/hidegroupdetail)(bool, int) | تصغير الصفوف / الأعمدة المجمعة. |
| [HideRow](../../aspose.cells/cells/hiderow)(int) | يخفي صفًا . |
| [HideRows](../../aspose.cells/cells/hiderows)(int, int) | إخفاء عدة صفوف . |
| [ImportArray](../../aspose.cells/cells/importarray#importarray)(double[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_2)(int[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_4)(string[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_1)(double[], int, int, bool) | يستورد مصفوفة مزدوجة في ورقة عمل. |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_3)(int[], int, int, bool) | يستورد مصفوفة من الأعداد الصحيحة في ورقة العمل. |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_5)(string[], int, int, bool) | يستورد مصفوفة سلسلة في ورقة عمل. |
| [ImportArrayList](../../aspose.cells/cells/importarraylist)(ArrayList, int, int, bool) | لاستيراد قائمة صفائف من البيانات في ورقة عمل. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv)(Stream, TxtLoadOptions, int, int) | استيراد ملف CSV إلى الخلايا. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv_2)(string, TxtLoadOptions, int, int) | استيراد ملف CSV إلى الخلايا. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv_1)(Stream, string, bool, int, int) | استيراد ملف CSV إلى الخلايا. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv_3)(string, string, bool, int, int) | استيراد ملف CSV إلى الخلايا. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects#importcustomobjects)(ICollection, int, int, ImportTableOptions) | استيراد الكائنات المخصصة. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects#importcustomobjects_1)(ICollection, string[], bool, int, int, int, bool, string, bool) | استيراد الكائنات المخصصة. |
| [ImportData](../../aspose.cells/cells/importdata#importdata_3)(IDataReader, int, int) | يستورد البيانات من ملفIDataReader الكائن . |
| [ImportData](../../aspose.cells/cells/importdata#importdata_1)(DataTable, int, int, ImportTableOptions) | استيراد البيانات من جدول البيانات المخصصة . |
| [ImportData](../../aspose.cells/cells/importdata#importdata_2)(DataView, int, int, ImportTableOptions) | استيراد البيانات من عرض البيانات . |
| [ImportData](../../aspose.cells/cells/importdata#importdata)(ICellsDataTable, int, int, ImportTableOptions) | استيراد البيانات من جدول البيانات المخصصة . |
| [ImportData](../../aspose.cells/cells/importdata#importdata_4)(IDataReader, int, int, ImportTableOptions) | يستورد البيانات من ملفIDataReader الكائن . |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid#importdatagrid)(DataGrid, int, int, bool) | الواردات أDataGrid في ورقة عمل. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid#importdatagrid_1)(DataGrid, int, int, int, int, bool) | الواردات أDataGrid في ورقة عمل. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid#importdatagrid_2)(DataGrid, int, int, int, int, bool, bool) | الواردات أDataGrid في ورقة عمل. |
| [ImportDataGridAsString](../../aspose.cells/cells/importdatagridasstring)(DataGrid, int, int, bool) | الواردات أDataGrid في ورقة عمل. لا تحاول هذه الطريقة تحويل النص إلى قيم رقمية. |
| [ImportDataRow](../../aspose.cells/cells/importdatarow)(DataRow, int, int) | يستورد DataRow إلى ملف Excel. |
| [ImportDataView](../../aspose.cells/cells/importdataview#importdataview_3)(DataView, int, int) | الواردات أDataView في ورقة عمل. |
| [ImportFormulaArray](../../aspose.cells/cells/importformulaarray)(string[], int, int, bool) | يستورد مصفوفة من الصيغة في ورقة عمل. |
| [ImportGridView](../../aspose.cells/cells/importgridview)(GridView, int, int, ImportTableOptions) | يستورد طريقة عرض الشبكة لهذه الخلايا. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray#importobjectarray)(object[], int, int, bool) | يستورد مصفوفة من البيانات في ورقة عمل. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray#importobjectarray_1)(object[], int, int, bool, int) | يستورد مصفوفة من البيانات في ورقة عمل. |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray)(object[], int, int) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray_1)(object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray_3)(object[], object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray_2)(object[], object[], int, int, TxtLoadOptions) |  |
| [InsertColumn](../../aspose.cells/cells/insertcolumn#insertcolumn)(int) | إدراج عمود جديد بورقة العمل. |
| [InsertColumn](../../aspose.cells/cells/insertcolumn#insertcolumn_1)(int, bool) | إدراج عمود جديد بورقة العمل. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns#insertcolumns)(int, int) | إدراج بعض الأعمدة في ورقة العمل. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns#insertcolumns_1)(int, int, bool) | إدراج بعض الأعمدة في ورقة العمل. |
| [InsertCutCells](../../aspose.cells/cells/insertcutcells)(Range, int, int, ShiftType) | أدخل نطاق القطع . |
| [InsertRange](../../aspose.cells/cells/insertrange#insertrange)(CellArea, ShiftType) | لإدراج نطاق من الخلايا وإزاحة الخلايا وفقًا لخيار الإزاحة. |
| [InsertRange](../../aspose.cells/cells/insertrange#insertrange_1)(CellArea, int, ShiftType) | لإدراج نطاق من الخلايا وإزاحة الخلايا وفقًا لخيار الإزاحة. |
| [InsertRange](../../aspose.cells/cells/insertrange#insertrange_2)(CellArea, int, ShiftType, bool) | لإدراج نطاق من الخلايا وإزاحة الخلايا وفقًا لخيار الإزاحة. |
| [InsertRow](../../aspose.cells/cells/insertrow)(int) | إدراج صف جديد في ورقة العمل . |
| [InsertRows](../../aspose.cells/cells/insertrows#insertrows)(int, int) | إدراج عدة صفوف في ورقة العمل . |
| [InsertRows](../../aspose.cells/cells/insertrows#insertrows_2)(int, int, bool) | إدراج عدة صفوف في ورقة العمل . |
| [InsertRows](../../aspose.cells/cells/insertrows#insertrows_1)(int, int, InsertOptions) | إدراج عدة صفوف في ورقة العمل . |
| [IsBlankColumn](../../aspose.cells/cells/isblankcolumn)(int) | للتحقق مما إذا كان العمود المحدد فارغًا (لا يحتوي على أي بيانات) . |
| [IsColumnHidden](../../aspose.cells/cells/iscolumnhidden)(int) | للتحقق مما إذا كان عمود في فهرس معين مخفيًا . |
| [IsDeletingRangeEnabled](../../aspose.cells/cells/isdeletingrangeenabled)(int, int, int, int) | تحقق مما إذا كان يمكن حذف النطاق. |
| [IsRowHidden](../../aspose.cells/cells/isrowhidden)(int) | للتحقق مما إذا كان صف في فهرس معين مخفيًا . |
| [LinkToXmlMap](../../aspose.cells/cells/linktoxmlmap)(string, int, int, string) | رابط لخريطة xml . |
| [Merge](../../aspose.cells/cells/merge#merge)(int, int, int, int) | يدمج نطاقًا محددًا من الخلايا في خلية واحدة. |
| [Merge](../../aspose.cells/cells/merge#merge_1)(int, int, int, int, bool) | يدمج نطاقًا محددًا من الخلايا في خلية واحدة. |
| [Merge](../../aspose.cells/cells/merge#merge_2)(int, int, int, int, bool, bool) | يدمج نطاقًا محددًا من الخلايا في خلية واحدة. |
| [MoveRange](../../aspose.cells/cells/moverange)(CellArea, int, int) | لنقل النطاق . |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates#removeduplicates)() | يزيل الصفوف المكررة من الورقة. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates#removeduplicates_1)(int, int, int, int) | يزيل القيم المكررة في النطاق . |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates#removeduplicates_2)(int, int, int, int, bool, int[]) | يزيل البيانات المكررة من النطاق. |
| [RemoveFormulas](../../aspose.cells/cells/removeformulas)() | يزيل كل الصيغة ويستبدل بقيمة الصيغة. |
| [RetrieveSubtotalSetting](../../aspose.cells/cells/retrievesubtotalsetting)(CellArea) | استرداد إعداد المجاميع الفرعية للنطاق. |
| [SetColumnWidth](../../aspose.cells/cells/setcolumnwidth)(int, double) | يضبط عرض العمود المحدد في العرض العادي. |
| [SetColumnWidthInch](../../aspose.cells/cells/setcolumnwidthinch)(int, double) | يضبط عرض العمود بوحدة البوصة في العرض العادي. |
| [SetColumnWidthPixel](../../aspose.cells/cells/setcolumnwidthpixel)(int, int) | يضبط عرض العمود بوحدة البكسل في العرض العادي. |
| [SetRowHeight](../../aspose.cells/cells/setrowheight)(int, double) | يحدد ارتفاع الصف المحدد. |
| [SetRowHeightInch](../../aspose.cells/cells/setrowheightinch)(int, double) | يضبط ارتفاع الصف بوحدة بوصة . |
| [SetRowHeightPixel](../../aspose.cells/cells/setrowheightpixel)(int, int) | يضبط ارتفاع الصف بوحدة البكسل . |
| [SetViewColumnWidthPixel](../../aspose.cells/cells/setviewcolumnwidthpixel)(int, int) | يضبط عرض العمود في طريقة عرض مختلفة. |
| [ShowGroupDetail](../../aspose.cells/cells/showgroupdetail)(bool, int) | يوسع الصفوف / الأعمدة المجمعة. |
| [Subtotal](../../aspose.cells/cells/subtotal#subtotal)(CellArea, int, ConsolidationFunction, int[]) | إنشاء مجاميع فرعية للنطاق . |
| [Subtotal](../../aspose.cells/cells/subtotal#subtotal_1)(CellArea, int, ConsolidationFunction, int[], bool, bool, bool) | إنشاء مجاميع فرعية للنطاق . |
| [TextToColumns](../../aspose.cells/cells/texttocolumns)(int, int, int, TxtLoadOptions) | لتقسيم النص في العمود إلى أعمدة . |
| [UngroupColumns](../../aspose.cells/cells/ungroupcolumns)(int, int) | فك تجميع الأعمدة. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows#ungrouprows)(int, int) | يفك تجميع الصفوف . |
| [UngroupRows](../../aspose.cells/cells/ungrouprows#ungrouprows_1)(int, int, bool) | يفك تجميع الصفوف . |
| [UnhideColumn](../../aspose.cells/cells/unhidecolumn)(int, double) | إظهار عمود |
| [UnhideColumns](../../aspose.cells/cells/unhidecolumns)(int, int, double) | إظهار عدة أعمدة. |
| [UnhideRow](../../aspose.cells/cells/unhiderow)(int, double) | إظهار صف . |
| [UnhideRows](../../aspose.cells/cells/unhiderows)(int, int, double) | إظهار الصفوف المخفية . |
| [UnMerge](../../aspose.cells/cells/unmerge)(int, int, int, int) | يدمج نطاقًا محددًا من الخلايا المدمجة. |

### أمثلة

```csharp

[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

// تعيين ارتفاع الصف الافتراضي
cells.StandardHeight = 20;
// تعيين ارتفاع الصف
cells.SetRowHeight(2, 20.5);

// تعيين عرض العمود الافتراضي
cells.StandardWidth = 15;
// ضبط عرض العمود
cells.SetColumnWidth(3, 12.57);

//دمج الخلايا
cells.Merge(5, 4, 2, 2);

// ضع القيم في الخلايا
cells[0, 0].PutValue(true);
cells[0, 1].PutValue(1);
cells[0, 2].PutValue("abc");

// تصدير البيانات
object[,] arr = cells.ExportArray(0, 0, 10, 10);

[Visual Basic]

Dim excel as Workbook = new Workbook()
Dim cells as Cells = excel.Worksheets(0).Cells

'تعيين ارتفاع الصف الافتراضي
cells.StandardHeight = 20
'تعيين ارتفاع الصف
cells.SetRowHeight(2, 20.5)

'تعيين عرض العمود الافتراضي
cells.StandardWidth = 15
'تعيين عرض العمود
cells.SetColumnWidth(3, 12.57)

'دمج الخلايا
cells.Merge(5, 4, 2, 2)

'تصدير البيانات
Dim outDataTable as DataTable = cells.ExportDataTable(12, 12, 10, 10)
```

### أنظر أيضا

* مساحة الاسم [Aspose.Cells](../../aspose.cells)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
