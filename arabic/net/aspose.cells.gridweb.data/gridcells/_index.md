---
title: GridCells
second_title: Aspose.Cells لمرجع .NET API
description: لتغليف مجموعة منCell الكائنات .
type: docs
weight: 190
url: /ar/net/aspose.cells.gridweb.data/gridcells/
---
## GridCells class

لتغليف مجموعة منCell الكائنات .

```csharp
public class GridCells : IEnumerable
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [Columns](../../aspose.cells.gridweb.data/gridcells/columns) { get; } |  |
| [Count](../../aspose.cells.gridweb.data/gridcells/count) { get; } | الحصول على عدد الخلايا . |
| [FirstCell](../../aspose.cells.gridweb.data/gridcells/firstcell) { get; } |  |
| [Item](../../aspose.cells.gridweb.data/gridcells/item) { get; } | يحصلCell عنصر داخل ورقة العمل (3 indexers) |
| [LastCell](../../aspose.cells.gridweb.data/gridcells/lastcell) { get; } |  |
| [MaxColumn](../../aspose.cells.gridweb.data/gridcells/maxcolumn) { get; } | الحد الأقصى لفهرس عمود الخلية الذي يحتوي على بيانات أو نمط . |
| [MaxDataColumn](../../aspose.cells.gridweb.data/gridcells/maxdatacolumn) { get; } |  |
| [MaxDataRow](../../aspose.cells.gridweb.data/gridcells/maxdatarow) { get; } |  |
| [MaxRow](../../aspose.cells.gridweb.data/gridcells/maxrow) { get; } | الحد الأقصى لفهرس صف الخلية الذي يحتوي على بيانات أو نمط . |
| [MergedCells](../../aspose.cells.gridweb.data/gridcells/mergedcells) { get; } | الحصول على مجموعة الخلايا المدمجة. |
| [MinColumn](../../aspose.cells.gridweb.data/gridcells/mincolumn) { get; } |  |
| [MinDataColumn](../../aspose.cells.gridweb.data/gridcells/mindatacolumn) { get; } |  |
| [MinDataRow](../../aspose.cells.gridweb.data/gridcells/mindatarow) { get; } |  |
| [MinRow](../../aspose.cells.gridweb.data/gridcells/minrow) { get; } |  |
| [RowEnumerator](../../aspose.cells.gridweb.data/gridcells/rowenumerator) { get; } | الحصول على عداد الصفوف |
| [Rows](../../aspose.cells.gridweb.data/gridcells/rows) { get; } |  |
| [StandardHeight](../../aspose.cells.gridweb.data/gridcells/standardheight) { get; set; } | الحصول على أو تعيين الارتفاع الافتراضي للصف في ورقة العمل هذه ، بوحدة النقاط. |
| [StandardHeightPixels](../../aspose.cells.gridweb.data/gridcells/standardheightpixels) { get; set; } | الحصول على أو تعيين الارتفاع الافتراضي للصف في ورقة العمل هذه ، بوحدة البكسل. |
| [StandardWidth](../../aspose.cells.gridweb.data/gridcells/standardwidth) { get; set; } | الحصول على أو تعيين عرض العمود الافتراضي في ورقة العمل ، في وحدة من الأحرف. |
| [StandardWidthInch](../../aspose.cells.gridweb.data/gridcells/standardwidthinch) { get; set; } |  |
| [StandardWidthPixels](../../aspose.cells.gridweb.data/gridcells/standardwidthpixels) { get; set; } |  |

## طُرق

| اسم | وصف |
| --- | --- |
| [Clear](../../aspose.cells.gridweb.data/gridcells/clear)() | مسح كافة الخلايا في المجموعة. |
| [ClearContents](../../aspose.cells.gridweb.data/gridcells/clearcontents#clearcontents)(GridCellArea) | يمسح محتويات النطاق . |
| [ClearContents](../../aspose.cells.gridweb.data/gridcells/clearcontents#clearcontents_1)(int, int, int, int) | يمسح محتويات النطاق . |
| [ClearFormats](../../aspose.cells.gridweb.data/gridcells/clearformats#clearformats)(GridCellArea) | مسح تنسيق النطاق. |
| [ClearFormats](../../aspose.cells.gridweb.data/gridcells/clearformats#clearformats_1)(int, int, int, int) | مسح تنسيق النطاق. |
| [ClearRange](../../aspose.cells.gridweb.data/gridcells/clearrange#clearrange)(GridCellArea) | يمسح محتويات وتنسيق النطاق. |
| [ClearRange](../../aspose.cells.gridweb.data/gridcells/clearrange#clearrange_1)(int, int, int, int) | يمسح محتويات وتنسيق النطاق. |
| [CopyColumn](../../aspose.cells.gridweb.data/gridcells/copycolumn)(GridCells, int, int) | نسخ البيانات وتنسيقات عمود كامل. |
| [CopyColumns](../../aspose.cells.gridweb.data/gridcells/copycolumns)(GridCells, int, int, int) | نسخ البيانات وتنسيقات عمود كامل. |
| [CopyRow](../../aspose.cells.gridweb.data/gridcells/copyrow)(GridCells, int, int) | نسخ البيانات وتنسيقات صف كامل. |
| [CopyRows](../../aspose.cells.gridweb.data/gridcells/copyrows)(GridCells, int, int, int) | نسخ البيانات والتنسيقات لبعض الصفوف بأكملها. |
| [DeleteBlankColumns](../../aspose.cells.gridweb.data/gridcells/deleteblankcolumns)() | احذف جميع الأعمدة الفارغة التي لا تحتوي على أي بيانات. |
| [DeleteBlankRows](../../aspose.cells.gridweb.data/gridcells/deleteblankrows)() | احذف جميع الصفوف الفارغة التي لا تحتوي على أي بيانات. |
| [DeleteColumn](../../aspose.cells.gridweb.data/gridcells/deletecolumn#deletecolumn)(int) | حذف عمود . |
| [DeleteColumn](../../aspose.cells.gridweb.data/gridcells/deletecolumn#deletecolumn_1)(int, bool) | حذف عمود . |
| [DeleteColumns](../../aspose.cells.gridweb.data/gridcells/deletecolumns)(int, int, bool) | حذف عدة أعمدة . |
| [DeleteRange](../../aspose.cells.gridweb.data/gridcells/deleterange)(int, int, int, int, GridShiftType) | حذف نطاق من الخلايا وإزاحة الخلايا وفقًا لخيار الإزاحة. |
| [DeleteRow](../../aspose.cells.gridweb.data/gridcells/deleterow)(int) | حذف صف . |
| [DeleteRows](../../aspose.cells.gridweb.data/gridcells/deleterows#deleterows)(int, int) | حذف عدة صفوف . |
| [DeleteRows](../../aspose.cells.gridweb.data/gridcells/deleterows#deleterows_1)(int, int, bool) | حذف عدة صفوف من ورقة العمل . |
| [Export](../../aspose.cells.gridweb.data/gridcells/export)(int, int, int, int, bool, bool) | تصدير البيانات في مجموعة الخلايا لورقة ويب إلى كائن DataTable جديد |
| [ExportArray](../../aspose.cells.gridweb.data/gridcells/exportarray)(int, int, int, int) | يتم تصدير البيانات بتنسيقCellsالمجموعة إلى كائن مصفوفة ثنائية الأبعاد. |
| [GetCell](../../aspose.cells.gridweb.data/gridcells/getcell)(int, int) | يحصل على ملفCell عنصر أو فارغ في فهرس صف الخلية المحدد وفهرس العمود. |
| [GetColumnWidth](../../aspose.cells.gridweb.data/gridcells/getcolumnwidth)(int) | الحصول على عرض العمود المحدد |
| [GetColumnWidthInch](../../aspose.cells.gridweb.data/gridcells/getcolumnwidthinch)(int) | الحصول على عرض العمود المحدد ، بوحدات البوصة . |
| [GetColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/getcolumnwidthpixel)(int) | الحصول على عرض العمود المحدد بوحدات البكسل. |
| [GetEnumerator](../../aspose.cells.gridweb.data/gridcells/getenumerator)() | الحصول على عداد الصفوف |
| [GetRow](../../aspose.cells.gridweb.data/gridcells/getrow)(int) | يحصل على ملفRow عنصر أو في فهرس صف الخلية المحدد. |
| [GetRowHeight](../../aspose.cells.gridweb.data/gridcells/getrowheight)(int) | الحصول على ارتفاع صف معين. |
| [GetRowHeightInch](../../aspose.cells.gridweb.data/gridcells/getrowheightinch)(int) | الحصول على ارتفاع صف محدد بوحدة البوصة . |
| [GetRowHeightPixel](../../aspose.cells.gridweb.data/gridcells/getrowheightpixel)(int) | الحصول على ارتفاع صف محدد بوحدة البكسل . |
| [GetRowOutlineLevel](../../aspose.cells.gridweb.data/gridcells/getrowoutlinelevel)(int) | يحصل على مستوى المخطط التفصيلي للصف . |
| [GetViewColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/getviewcolumnwidthpixel)(int) | احصل على العرض بنوع عرض مختلف . |
| [GroupColumns](../../aspose.cells.gridweb.data/gridcells/groupcolumns#groupcolumns)(int, int) | أعمدة المجموعات. |
| [GroupColumns](../../aspose.cells.gridweb.data/gridcells/groupcolumns#groupcolumns_1)(int, int, bool) | أعمدة المجموعات. |
| [GroupRows](../../aspose.cells.gridweb.data/gridcells/grouprows)(int, int) | صفوف المجموعات . |
| [HideColumn](../../aspose.cells.gridweb.data/gridcells/hidecolumn)(int) | إخفاء عمود . |
| [HideRow](../../aspose.cells.gridweb.data/gridcells/hiderow)(int) | يخفي صفًا . |
| [InsertColumn](../../aspose.cells.gridweb.data/gridcells/insertcolumn#insertcolumn)(int) | إدراج عمود جديد بورقة العمل. |
| [InsertColumn](../../aspose.cells.gridweb.data/gridcells/insertcolumn#insertcolumn_1)(int, bool) | إدراج عمود جديد بورقة العمل. |
| [InsertColumns](../../aspose.cells.gridweb.data/gridcells/insertcolumns#insertcolumns)(int, int) | إدراج بعض الأعمدة في ورقة العمل. |
| [InsertColumns](../../aspose.cells.gridweb.data/gridcells/insertcolumns#insertcolumns_1)(int, int, bool) | إدراج بعض الأعمدة في ورقة العمل. |
| [InsertRange](../../aspose.cells.gridweb.data/gridcells/insertrange#insertrange)(GridCellArea, GridShiftType) | لإدراج نطاق من الخلايا وإزاحة الخلايا وفقًا لخيار الإزاحة. |
| [InsertRange](../../aspose.cells.gridweb.data/gridcells/insertrange#insertrange_1)(GridCellArea, int, GridShiftType, bool) | لإدراج نطاق من الخلايا وإزاحة الخلايا وفقًا لخيار الإزاحة. |
| [InsertRow](../../aspose.cells.gridweb.data/gridcells/insertrow)(int) | إدراج صف جديد في ورقة العمل . |
| [InsertRows](../../aspose.cells.gridweb.data/gridcells/insertrows#insertrows)(int, int) | إدراج عدة صفوف في ورقة العمل . |
| [InsertRows](../../aspose.cells.gridweb.data/gridcells/insertrows#insertrows_1)(int, int, bool) | إدراج عدة صفوف في ورقة العمل . |
| [IsBlankColumn](../../aspose.cells.gridweb.data/gridcells/isblankcolumn)(int) | للتحقق مما إذا كان العمود المحدد فارغًا (لا يحتوي على أي بيانات) . |
| [IsColumnHidden](../../aspose.cells.gridweb.data/gridcells/iscolumnhidden)(int) | للتحقق مما إذا كان عمود في فهرس معين مخفيًا . |
| [IsRowHidden](../../aspose.cells.gridweb.data/gridcells/isrowhidden)(int) | للتحقق مما إذا كان صف في فهرس معين مخفيًا . |
| [Merge](../../aspose.cells.gridweb.data/gridcells/merge)(int, int, int, int) | يدمج نطاقًا محددًا من الخلايا في خلية واحدة. |
| [MoveRange](../../aspose.cells.gridweb.data/gridcells/moverange)(GridCellArea, int, int) | لنقل النطاق . |
| [RemoveFormulas](../../aspose.cells.gridweb.data/gridcells/removeformulas)() | يزيل كل الصيغة ويستبدل بقيمة الصيغة. |
| [SetBorders](../../aspose.cells.gridweb.data/gridcells/setborders)(int, int, int, int, SetBorderPosition, WebBorderStyle) | تعيين الحدود لنطاق من الخلايا . |
| [SetColumnWidth](../../aspose.cells.gridweb.data/gridcells/setcolumnwidth)(int, double) | يضبط عرض العمود المحدد. |
| [SetColumnWidthInch](../../aspose.cells.gridweb.data/gridcells/setcolumnwidthinch)(int, double) | يضبط عرض العمود بوحدة البوصة . |
| [SetColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/setcolumnwidthpixel)(int, int) | يضبط عرض العمود بوحدة البكسل . |
| [SetRowHeight](../../aspose.cells.gridweb.data/gridcells/setrowheight)(int, double) | يحدد ارتفاع الصف المحدد. |
| [SetRowHeightInch](../../aspose.cells.gridweb.data/gridcells/setrowheightinch)(int, double) | يضبط ارتفاع الصف بوحدة بوصة . |
| [SetRowHeightPixel](../../aspose.cells.gridweb.data/gridcells/setrowheightpixel)(int, int) | يضبط ارتفاع الصف بوحدة البكسل . |
| [SetRowOutlineLevel](../../aspose.cells.gridweb.data/gridcells/setrowoutlinelevel)(int, int) | يضبط مستوى المخطط التفصيلي للصف . |
| [SetStyle](../../aspose.cells.gridweb.data/gridcells/setstyle#setstyle_1)(string, GridTableItemStyle) | يضبط النمط على نطاق محدد من الخلايا . |
| [SetStyle](../../aspose.cells.gridweb.data/gridcells/setstyle#setstyle)(int, int, int, int, GridTableItemStyle) | يضبط النمط على نطاق محدد من الخلايا . |
| [Sort](../../aspose.cells.gridweb.data/gridcells/sort#sort)(int, int, int, int, int, bool, bool, bool) | يفرز البيانات تصاعديًا / تنازليًا من أعلى إلى أسفل في نطاق من ورقة العمل حسب فهرس العمود المحدد. |
| [Sort](../../aspose.cells.gridweb.data/gridcells/sort#sort_1)(int, int, int, int, int[], SortOrder[], SortOrientation, bool) |  |
| [UngroupColumns](../../aspose.cells.gridweb.data/gridcells/ungroupcolumns)(int, int) | فك تجميع الأعمدة. |
| [UngroupRows](../../aspose.cells.gridweb.data/gridcells/ungrouprows)(int, int) | يفك تجميع الصفوف . |
| [UnhideColumn](../../aspose.cells.gridweb.data/gridcells/unhidecolumn)(int, double) | إظهار عمود |
| [UnhideRow](../../aspose.cells.gridweb.data/gridcells/unhiderow)(int) | إظهار صف . |
| [UnMerge](../../aspose.cells.gridweb.data/gridcells/unmerge)(int, int, int, int) | يدمج نطاقًا محددًا من الخلايا المدمجة. |
| static [CellIndexToName](../../aspose.cells.gridweb.data/gridcells/cellindextoname)(int, int) | الحصول على اسم الخلية وفقًا لفهارس الصفوف والأعمدة. |
| static [CellNameToIndex](../../aspose.cells.gridweb.data/gridcells/cellnametoindex)(string, out int, out int) | الحصول على فهارس صف الخلية والأعمدة وفقًا لاسمها |
| static [ColumnIndexToName](../../aspose.cells.gridweb.data/gridcells/columnindextoname)(int) | الحصول على اسم العمود وفقًا لفهرس العمود. |
| static [ColumnNameToIndex](../../aspose.cells.gridweb.data/gridcells/columnnametoindex)(string) | يحصل على فهرس العمود وفقًا لاسم العمود . |

### أنظر أيضا

* مساحة الاسم [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* المجسم [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
