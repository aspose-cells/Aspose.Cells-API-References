---
title: GridCells
second_title: Aspose.Cells لمرجع .NET API
description: لتغليف مجموعة منCellالكائنات .
type: docs
weight: 410
url: /ar/net/aspose.cells.griddesktop.data/gridcells/
---
## GridCells class

لتغليف مجموعة منCellالكائنات .

```csharp
public class GridCells : IEnumerable
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [Columns](../../aspose.cells.griddesktop.data/gridcells/columns) { get; } |  |
| [Count](../../aspose.cells.griddesktop.data/gridcells/count) { get; } | الحصول على عدد الخلايا . |
| [FirstCell](../../aspose.cells.griddesktop.data/gridcells/firstcell) { get; } |  |
| [Item](../../aspose.cells.griddesktop.data/gridcells/item) { get; } | يحصلCell عنصر داخل ورقة العمل (3 indexers) |
| [LastCell](../../aspose.cells.griddesktop.data/gridcells/lastcell) { get; } |  |
| [MaxColumn](../../aspose.cells.griddesktop.data/gridcells/maxcolumn) { get; } | الحد الأقصى لفهرس عمود الخلية الذي يحتوي على بيانات أو نمط . |
| [MaxDataColumn](../../aspose.cells.griddesktop.data/gridcells/maxdatacolumn) { get; } |  |
| [MaxDataRow](../../aspose.cells.griddesktop.data/gridcells/maxdatarow) { get; } |  |
| [MaxRow](../../aspose.cells.griddesktop.data/gridcells/maxrow) { get; } | الحد الأقصى لفهرس صف الخلية الذي يحتوي على بيانات أو نمط . |
| [MergedCells](../../aspose.cells.griddesktop.data/gridcells/mergedcells) { get; } | الحصول على مجموعة الخلايا المدمجة. |
| [MinColumn](../../aspose.cells.griddesktop.data/gridcells/mincolumn) { get; } |  |
| [MinDataColumn](../../aspose.cells.griddesktop.data/gridcells/mindatacolumn) { get; } |  |
| [MinDataRow](../../aspose.cells.griddesktop.data/gridcells/mindatarow) { get; } |  |
| [MinRow](../../aspose.cells.griddesktop.data/gridcells/minrow) { get; } |  |
| [RowEnumerator](../../aspose.cells.griddesktop.data/gridcells/rowenumerator) { get; } | الحصول على عداد الصفوف |
| [Rows](../../aspose.cells.griddesktop.data/gridcells/rows) { get; } | يحصل على مجموعة[`GridRow`](../gridrow) كائنات تمثل الصفوف الفردية في ورقة العمل هذه. |
| [StandardHeight](../../aspose.cells.griddesktop.data/gridcells/standardheight) { get; set; } | الحصول على أو تعيين الارتفاع الافتراضي للصف في ورقة العمل هذه ، بوحدة النقاط. |
| [StandardHeightPixels](../../aspose.cells.griddesktop.data/gridcells/standardheightpixels) { get; set; } | الحصول على أو تعيين الارتفاع الافتراضي للصف في ورقة العمل هذه ، بوحدة البكسل. |
| [StandardWidth](../../aspose.cells.griddesktop.data/gridcells/standardwidth) { get; set; } | الحصول على أو تعيين عرض العمود الافتراضي في ورقة العمل ، في وحدة من الأحرف. |
| [StandardWidthInch](../../aspose.cells.griddesktop.data/gridcells/standardwidthinch) { get; set; } |  |
| [StandardWidthPixels](../../aspose.cells.griddesktop.data/gridcells/standardwidthpixels) { get; set; } |  |

## طُرق

| اسم | وصف |
| --- | --- |
| [CheckCell](../../aspose.cells.griddesktop.data/gridcells/checkcell)(int, int) | يحصل على ملفCell عنصر أو فارغ في فهرس صف الخلية المحدد وفهرس العمود. |
| [Clear](../../aspose.cells.griddesktop.data/gridcells/clear)() | مسح كافة الخلايا في المجموعة. |
| [ClearContents](../../aspose.cells.griddesktop.data/gridcells/clearcontents#clearcontents)(GridCellArea) | يمسح محتويات النطاق . |
| [ClearContents](../../aspose.cells.griddesktop.data/gridcells/clearcontents#clearcontents_1)(int, int, int, int) | يمسح محتويات النطاق . |
| [ClearFormats](../../aspose.cells.griddesktop.data/gridcells/clearformats#clearformats)(GridCellArea) | مسح تنسيق النطاق. |
| [ClearFormats](../../aspose.cells.griddesktop.data/gridcells/clearformats#clearformats_1)(int, int, int, int) | مسح تنسيق النطاق. |
| [ClearRange](../../aspose.cells.griddesktop.data/gridcells/clearrange#clearrange)(GridCellArea) | يمسح محتويات وتنسيق النطاق. |
| [ClearRange](../../aspose.cells.griddesktop.data/gridcells/clearrange#clearrange_1)(int, int, int, int) | يمسح محتويات وتنسيق النطاق. |
| [CopyColumn](../../aspose.cells.griddesktop.data/gridcells/copycolumn)(GridCells, int, int) | نسخ البيانات وتنسيقات عمود كامل. |
| [CopyColumns](../../aspose.cells.griddesktop.data/gridcells/copycolumns)(GridCells, int, int, int) | نسخ البيانات وتنسيقات عمود كامل. |
| [CopyRow](../../aspose.cells.griddesktop.data/gridcells/copyrow)(GridCells, int, int) | نسخ البيانات وتنسيقات صف كامل. |
| [CopyRows](../../aspose.cells.griddesktop.data/gridcells/copyrows)(GridCells, int, int, int) | نسخ البيانات والتنسيقات لبعض الصفوف بأكملها. |
| [DeleteBlankColumns](../../aspose.cells.griddesktop.data/gridcells/deleteblankcolumns)() | احذف جميع الأعمدة الفارغة التي لا تحتوي على أي بيانات. |
| [DeleteBlankRows](../../aspose.cells.griddesktop.data/gridcells/deleteblankrows)() | احذف جميع الصفوف الفارغة التي لا تحتوي على أي بيانات. |
| [DeleteColumn](../../aspose.cells.griddesktop.data/gridcells/deletecolumn#deletecolumn)(int) | حذف عمود . |
| [DeleteColumn](../../aspose.cells.griddesktop.data/gridcells/deletecolumn#deletecolumn_1)(int, bool) | حذف عمود . |
| [DeleteColumns](../../aspose.cells.griddesktop.data/gridcells/deletecolumns)(int, int, bool) | حذف عدة أعمدة . |
| [DeleteRow](../../aspose.cells.griddesktop.data/gridcells/deleterow)(int) | حذف صف . |
| [DeleteRows](../../aspose.cells.griddesktop.data/gridcells/deleterows#deleterows)(int, int) | حذف عدة صفوف . |
| [DeleteRows](../../aspose.cells.griddesktop.data/gridcells/deleterows#deleterows_1)(int, int, bool) | حذف عدة صفوف من ورقة العمل . |
| [GetCell](../../aspose.cells.griddesktop.data/gridcells/getcell)(int, int) | يحصل على ملفCell عنصر أو فارغ في فهرس صف الخلية المحدد وفهرس العمود. |
| [GetCellStyle](../../aspose.cells.griddesktop.data/gridcells/getcellstyle)(int, int) | احصل على نمط الخلية المحددة . |
| [GetColumn](../../aspose.cells.griddesktop.data/gridcells/getcolumn)(int) | يحصل على ملف[`GridColumn`](../gridcolumn) عنصر أو في فهرس عمود الخلية المحدد. |
| [GetColumnWidth](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidth)(int) | الحصول على عرض العمود المحدد |
| [GetColumnWidthInch](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidthinch)(int) | الحصول على عرض العمود المحدد ، بوحدات البوصة . |
| [GetColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidthpixel)(int) | الحصول على عرض العمود المحدد بوحدات البكسل. |
| [GetEnumerator](../../aspose.cells.griddesktop.data/gridcells/getenumerator)() | الحصول على عداد الصفوف |
| [GetRow](../../aspose.cells.griddesktop.data/gridcells/getrow)(int) | يحصل على ملف[`GridRow`](../gridrow) عنصر أو في فهرس صف الخلية المحدد. |
| [GetRowHeight](../../aspose.cells.griddesktop.data/gridcells/getrowheight)(int) | الحصول على ارتفاع صف معين. |
| [GetRowHeightInch](../../aspose.cells.griddesktop.data/gridcells/getrowheightinch)(int) | الحصول على ارتفاع صف محدد بوحدة البوصة . |
| [GetRowHeightPixel](../../aspose.cells.griddesktop.data/gridcells/getrowheightpixel)(int) | الحصول على ارتفاع صف محدد بوحدة البكسل . |
| [GetViewColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/getviewcolumnwidthpixel)(int) | احصل على العرض بنوع عرض مختلف . |
| [GroupColumns](../../aspose.cells.griddesktop.data/gridcells/groupcolumns#groupcolumns)(int, int) | أعمدة المجموعات. |
| [GroupColumns](../../aspose.cells.griddesktop.data/gridcells/groupcolumns#groupcolumns_1)(int, int, bool) | أعمدة المجموعات. |
| [GroupRows](../../aspose.cells.griddesktop.data/gridcells/grouprows)(int, int) | صفوف المجموعات . |
| [HideColumn](../../aspose.cells.griddesktop.data/gridcells/hidecolumn)(int) | إخفاء عمود . |
| [HideRow](../../aspose.cells.griddesktop.data/gridcells/hiderow)(int) | يخفي صفًا . |
| [InsertColumn](../../aspose.cells.griddesktop.data/gridcells/insertcolumn#insertcolumn)(int) | إدراج عمود جديد بورقة العمل. |
| [InsertColumn](../../aspose.cells.griddesktop.data/gridcells/insertcolumn#insertcolumn_1)(int, bool) | إدراج عمود جديد بورقة العمل. |
| [InsertColumns](../../aspose.cells.griddesktop.data/gridcells/insertcolumns#insertcolumns)(int, int) | إدراج بعض الأعمدة في ورقة العمل. |
| [InsertColumns](../../aspose.cells.griddesktop.data/gridcells/insertcolumns#insertcolumns_1)(int, int, bool) | إدراج بعض الأعمدة في ورقة العمل. |
| [InsertRow](../../aspose.cells.griddesktop.data/gridcells/insertrow)(int) | إدراج صف جديد في ورقة العمل . |
| [InsertRows](../../aspose.cells.griddesktop.data/gridcells/insertrows#insertrows)(int, int) | إدراج عدة صفوف في ورقة العمل . |
| [InsertRows](../../aspose.cells.griddesktop.data/gridcells/insertrows#insertrows_1)(int, int, bool) | إدراج عدة صفوف في ورقة العمل . |
| [IsBlankColumn](../../aspose.cells.griddesktop.data/gridcells/isblankcolumn)(int) | للتحقق مما إذا كان العمود المحدد فارغًا (لا يحتوي على أي بيانات) . |
| [IsColumnHidden](../../aspose.cells.griddesktop.data/gridcells/iscolumnhidden)(int) | للتحقق مما إذا كان عمود في فهرس معين مخفيًا . |
| [IsRowHidden](../../aspose.cells.griddesktop.data/gridcells/isrowhidden)(int) | للتحقق مما إذا كان صف في فهرس معين مخفيًا . |
| [Merge](../../aspose.cells.griddesktop.data/gridcells/merge)(int, int, int, int) | يدمج نطاقًا محددًا من الخلايا في خلية واحدة. |
| [RemoveFormulas](../../aspose.cells.griddesktop.data/gridcells/removeformulas)() | يزيل كل الصيغة ويستبدل بقيمة الصيغة. |
| [SetColumnWidth](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidth)(int, double) | يضبط عرض العمود المحدد. |
| [SetColumnWidthInch](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidthinch)(int, double) | يضبط عرض العمود بوحدة البوصة . |
| [SetColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidthpixel)(int, int) | يضبط عرض العمود بوحدة البكسل . |
| [SetRowHeight](../../aspose.cells.griddesktop.data/gridcells/setrowheight)(int, double) | يحدد ارتفاع الصف المحدد. |
| [SetRowHeightInch](../../aspose.cells.griddesktop.data/gridcells/setrowheightinch)(int, double) | يضبط ارتفاع الصف بوحدة بوصة . |
| [SetRowHeightPixel](../../aspose.cells.griddesktop.data/gridcells/setrowheightpixel)(int, int) | يضبط ارتفاع الصف بوحدة البكسل . |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle#setstyle)(CellRange, Style) | يضبط النمط على نطاق محدد من الخلايا . |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle#setstyle_2)(string, Style) | يضبط النمط على نطاق محدد من الخلايا . |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle#setstyle_1)(int, int, int, int, Style) | يضبط النمط على نطاق محدد من الخلايا . |
| [Sort](../../aspose.cells.griddesktop.data/gridcells/sort#sort)(int, int, int, int, int, bool, bool, bool) | يفرز البيانات تصاعديًا / تنازليًا من أعلى إلى أسفل في نطاق من ورقة العمل حسب فهرس العمود المحدد. |
| [Sort](../../aspose.cells.griddesktop.data/gridcells/sort#sort_1)(int, int, int, int, int[], SortOrder[], SortOrientation, bool) |  |
| [UngroupColumns](../../aspose.cells.griddesktop.data/gridcells/ungroupcolumns)(int, int) | فك تجميع الأعمدة. |
| [UngroupRows](../../aspose.cells.griddesktop.data/gridcells/ungrouprows)(int, int) | يفك تجميع الصفوف . |
| [UnhideColumn](../../aspose.cells.griddesktop.data/gridcells/unhidecolumn)(int, double) | إظهار عمود |
| [UnhideRow](../../aspose.cells.griddesktop.data/gridcells/unhiderow)(int) | إظهار صف . |
| [UnMerge](../../aspose.cells.griddesktop.data/gridcells/unmerge)(int, int, int, int) | يدمج نطاقًا محددًا من الخلايا المدمجة. |
| static [CellIndexToName](../../aspose.cells.griddesktop.data/gridcells/cellindextoname)(int, int) | الحصول على اسم الخلية وفقًا لفهارس الصفوف والأعمدة. |
| static [CellNameToIndex](../../aspose.cells.griddesktop.data/gridcells/cellnametoindex)(string, out int, out int) | الحصول على فهارس صف الخلية والأعمدة وفقًا لاسمها |
| static [ColumnIndexToName](../../aspose.cells.griddesktop.data/gridcells/columnindextoname)(int) | الحصول على اسم العمود وفقًا لفهرس العمود. |
| static [ColumnNameToIndex](../../aspose.cells.griddesktop.data/gridcells/columnnametoindex)(string) | يحصل على فهرس العمود وفقًا لاسم العمود . |

### أنظر أيضا

* مساحة الاسم [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data)
* المجسم [Aspose.Cells.GridDesktop](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
