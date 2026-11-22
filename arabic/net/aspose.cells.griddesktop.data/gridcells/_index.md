---
title: "الفئة GridCells"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.GridDesktop.Data.GridCells. تغلف مجموعة من كائنات Cell"
type: docs
url: /ar/net/aspose.cells.griddesktop.data/gridcells/
---
## GridCells class

يغلف مجموعة من كائنات Cell.

```csharp
public class GridCells : IEnumerable
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Columns](../../aspose.cells.griddesktop.data/gridcells/columns/) { get; } |  |
| [Count](../../aspose.cells.griddesktop.data/gridcells/count/) { get; } | يحصل على عدد الخلايا. |
| [FirstCell](../../aspose.cells.griddesktop.data/gridcells/firstcell/) { get; } | يحصل على الخلية الأولى في ورقة العمل هذه. |
| [Item](../../aspose.cells.griddesktop.data/gridcells/item/) { get; } | يحصل على العنصر [`GridCell`](../gridcell/) في فهرس صف الخلية المحدد وفهرس العمود المحدد. (مؤشرين) |
| [LastCell](../../aspose.cells.griddesktop.data/gridcells/lastcell/) { get; } | يحصل على الخلية الأخيرة في ورقة العمل هذه. |
| [MaxColumn](../../aspose.cells.griddesktop.data/gridcells/maxcolumn/) { get; } | الحد الأقصى لفهرس العمود للخلية التي تحتوي على بيانات أو نمط. |
| [MaxDataColumn](../../aspose.cells.griddesktop.data/gridcells/maxdatacolumn/) { get; } | الحد الأقصى لفهرس العمود للخلية التي تحتوي على بيانات. |
| [MaxDataRow](../../aspose.cells.griddesktop.data/gridcells/maxdatarow/) { get; } | الحد الأقصى لفهرس الصف للخلية التي تحتوي على بيانات. |
| [MaxRow](../../aspose.cells.griddesktop.data/gridcells/maxrow/) { get; } | الحد الأقصى لفهرس الصف للخلية التي تحتوي على بيانات أو نمط. |
| [MergedCells](../../aspose.cells.griddesktop.data/gridcells/mergedcells/) { get; } | يحصل على مجموعة الخلايا المدمجة. |
| [MinColumn](../../aspose.cells.griddesktop.data/gridcells/mincolumn/) { get; } | الحد الأدنى لفهرس العمود لتلك الخلايا التي تم إنشاؤها في المجموعة (لا تشمل العمود الذي تم تعريف النمط له للعمود بأكمله ولكن لم يتم إنشاء أي خلية فيه). |
| [MinDataColumn](../../aspose.cells.griddesktop.data/gridcells/mindatacolumn/) { get; } | الحد الأدنى لفهرس العمود للخلية التي تحتوي على بيانات. |
| [MinDataRow](../../aspose.cells.griddesktop.data/gridcells/mindatarow/) { get; } | الحد الأدنى لمؤشر الصف للخلية التي تحتوي على بيانات. |
| [MinRow](../../aspose.cells.griddesktop.data/gridcells/minrow/) { get; } | الحد الأدنى لمؤشر الصف للخلية التي تحتوي على بيانات أو نمط. |
| [RowEnumerator](../../aspose.cells.griddesktop.data/gridcells/rowenumerator/) { get; } | يحصل على مُعدِّد الصفوف |
| [Rows](../../aspose.cells.griddesktop.data/gridcells/rows/) { get; } | يحصل على مجموعة كائنات [`GridRow`](../gridrow/) التي تمثل الصفوف الفردية في ورقة العمل هذه. |
| [StandardHeight](../../aspose.cells.griddesktop.data/gridcells/standardheight/) { get; set; } | يحصل أو يضبط ارتفاع الصف الافتراضي في ورقة العمل هذه، بوحدة النقاط. |
| [StandardHeightPixels](../../aspose.cells.griddesktop.data/gridcells/standardheightpixels/) { get; set; } | يحصل أو يضبط ارتفاع الصف الافتراضي في ورقة العمل هذه، بوحدة البكسل. |
| [StandardWidth](../../aspose.cells.griddesktop.data/gridcells/standardwidth/) { get; set; } | يحصل أو يضبط عرض العمود الافتراضي في ورقة العمل، بوحدة الأحرف. |
| [StandardWidthInch](../../aspose.cells.griddesktop.data/gridcells/standardwidthinch/) { get; set; } |  |
| [StandardWidthPixels](../../aspose.cells.griddesktop.data/gridcells/standardwidthpixels/) { get; set; } |  |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [CheckCell](../../aspose.cells.griddesktop.data/gridcells/checkcell/)(int, int) | يحصل على العنصر [`GridCell`](../gridcell/) أو null في فهرس صف الخلية المحدد وفهرس العمود المحدد. |
| [CheckRow](../../aspose.cells.griddesktop.data/gridcells/checkrow/)(int) | يحصل على العنصر [`GridRow`](../gridrow/) أو null في فهرس صف الخلية المحدد. |
| [Clear](../../aspose.cells.griddesktop.data/gridcells/clear/)() | امسح جميع الخلايا في المجموعة. |
| [ClearContents](../../aspose.cells.griddesktop.data/gridcells/clearcontents/#clearcontents)(GridCellArea) | يمسح محتويات نطاق. |
| [ClearContents](../../aspose.cells.griddesktop.data/gridcells/clearcontents/#clearcontents_1)(int, int, int, int) | يمسح محتويات نطاق. |
| [ClearFormats](../../aspose.cells.griddesktop.data/gridcells/clearformats/#clearformats)(GridCellArea) | يمسح تنسيق نطاق. |
| [ClearFormats](../../aspose.cells.griddesktop.data/gridcells/clearformats/#clearformats_1)(int, int, int, int) | يمسح تنسيق نطاق. |
| [ClearRange](../../aspose.cells.griddesktop.data/gridcells/clearrange/#clearrange)(GridCellArea) | يمسح محتويات وتنسيق نطاق. |
| [ClearRange](../../aspose.cells.griddesktop.data/gridcells/clearrange/#clearrange_1)(int, int, int, int) | يمسح محتويات وتنسيق نطاق. |
| [CopyColumn](../../aspose.cells.griddesktop.data/gridcells/copycolumn/)(GridCells, int, int) | ينسخ البيانات والتنسيقات لعمود كامل. |
| [CopyColumns](../../aspose.cells.griddesktop.data/gridcells/copycolumns/)(GridCells, int, int, int) | ينسخ البيانات والتنسيقات لعمود كامل. |
| [CopyRow](../../aspose.cells.griddesktop.data/gridcells/copyrow/)(GridCells, int, int) | ينسخ البيانات والتنسيقات لصف كامل. |
| [CopyRows](../../aspose.cells.griddesktop.data/gridcells/copyrows/)(GridCells, int, int, int) | ينسخ البيانات والتنسيقات لبعض الصفوف الكاملة. |
| [DeleteBlankColumns](../../aspose.cells.griddesktop.data/gridcells/deleteblankcolumns/)() | احذف جميع الأعمدة الفارغة التي لا تحتوي على أي بيانات. |
| [DeleteBlankRows](../../aspose.cells.griddesktop.data/gridcells/deleteblankrows/)() | احذف جميع الصفوف الفارغة التي لا تحتوي على أي بيانات. |
| [DeleteColumn](../../aspose.cells.griddesktop.data/gridcells/deletecolumn/#deletecolumn)(int) | يحذف عمودًا. |
| [DeleteColumn](../../aspose.cells.griddesktop.data/gridcells/deletecolumn/#deletecolumn_1)(int, bool) | يحذف عمودًا. |
| [DeleteColumns](../../aspose.cells.griddesktop.data/gridcells/deletecolumns/)(int, int, bool) | يحذف عدة أعمدة. |
| [DeleteRow](../../aspose.cells.griddesktop.data/gridcells/deleterow/)(int) | يحذف صفًا. |
| [DeleteRows](../../aspose.cells.griddesktop.data/gridcells/deleterows/#deleterows)(int, int) | يحذف عدة صفوف. |
| [DeleteRows](../../aspose.cells.griddesktop.data/gridcells/deleterows/#deleterows_1)(int, int, bool) | يحذف عدة صفوف في ورقة العمل. |
| [GetCellStyle](../../aspose.cells.griddesktop.data/gridcells/getcellstyle/)(int, int) | احصل على نمط الخلية المعطاة. |
| [GetColumn](../../aspose.cells.griddesktop.data/gridcells/getcolumn/)(int) | يحصل على العنصر [`GridColumn`](../gridcolumn/) أو في فهرس عمود الخلية المحدد. |
| [GetColumnWidth](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidth/)(int) | يحصل على عرض العمود المحدد |
| [GetColumnWidthInch](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidthinch/)(int) | يحصل على عرض العمود المحدد، بوحدة البوصة. |
| [GetColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidthpixel/)(int) | يحصل على عرض العمود المحدد، بوحدة البكسل. |
| [GetEnumerator](../../aspose.cells.griddesktop.data/gridcells/getenumerator/)() | يحصل على مُعدِّد الصفوف |
| [GetRow](../../aspose.cells.griddesktop.data/gridcells/getrow/)(int) | يحصل على العنصر [`GridRow`](../gridrow/) أو في فهرس صف الخلية المحدد. |
| [GetRowHeight](../../aspose.cells.griddesktop.data/gridcells/getrowheight/)(int) | يحصل على ارتفاع الصف المحدد. |
| [GetRowHeightInch](../../aspose.cells.griddesktop.data/gridcells/getrowheightinch/)(int) | يحصل على ارتفاع صف محدد بوحدة البوصة. |
| [GetRowHeightPixel](../../aspose.cells.griddesktop.data/gridcells/getrowheightpixel/)(int) | يحصل على ارتفاع الصف المحدد بوحدة البكسل. |
| [GetViewColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/getviewcolumnwidthpixel/)(int) | احصل على العرض في نوع عرض مختلف. |
| [GroupColumns](../../aspose.cells.griddesktop.data/gridcells/groupcolumns/#groupcolumns)(int, int) | يقوم بتجميع الأعمدة. |
| [GroupColumns](../../aspose.cells.griddesktop.data/gridcells/groupcolumns/#groupcolumns_1)(int, int, bool) | يقوم بتجميع الأعمدة. |
| [GroupRows](../../aspose.cells.griddesktop.data/gridcells/grouprows/)(int, int) | يقوم بتجميع الصفوف. |
| [HideColumn](../../aspose.cells.griddesktop.data/gridcells/hidecolumn/)(int) | يخفي عمودًا. |
| [HideColumns](../../aspose.cells.griddesktop.data/gridcells/hidecolumns/)(int, int) | إخفاء أعمدة متعددة. |
| [HideRow](../../aspose.cells.griddesktop.data/gridcells/hiderow/)(int) | يخفي صفًا. |
| [HideRows](../../aspose.cells.griddesktop.data/gridcells/hiderows/)(int, int) | يخفي صفوفًا متعددة. |
| [InsertColumn](../../aspose.cells.griddesktop.data/gridcells/insertcolumn/#insertcolumn)(int) | يدرج عمودًا جديدًا في ورقة العمل. |
| [InsertColumn](../../aspose.cells.griddesktop.data/gridcells/insertcolumn/#insertcolumn_1)(int, bool) | يدرج عمودًا جديدًا في ورقة العمل. |
| [InsertColumns](../../aspose.cells.griddesktop.data/gridcells/insertcolumns/#insertcolumns)(int, int) | يدرج بعض الأعمدة في ورقة العمل. |
| [InsertColumns](../../aspose.cells.griddesktop.data/gridcells/insertcolumns/#insertcolumns_1)(int, int, bool) | يدرج بعض الأعمدة في ورقة العمل. |
| [InsertRow](../../aspose.cells.griddesktop.data/gridcells/insertrow/)(int) | يدرج صفًا جديدًا في ورقة العمل. |
| [InsertRows](../../aspose.cells.griddesktop.data/gridcells/insertrows/#insertrows)(int, int) | يدرج عدة صفوف في ورقة العمل. |
| [InsertRows](../../aspose.cells.griddesktop.data/gridcells/insertrows/#insertrows_1)(int, int, bool) | يدرج عدة صفوف في ورقة العمل. |
| [IsBlankColumn](../../aspose.cells.griddesktop.data/gridcells/isblankcolumn/)(int) | يتحقق مما إذا كان العمود المحدد فارغًا (لا يحتوي على أي بيانات). |
| [IsColumnHidden](../../aspose.cells.griddesktop.data/gridcells/iscolumnhidden/)(int) | يتحقق مما إذا كان العمود في الفهرس المحدد مخفيًا. |
| [IsRowHidden](../../aspose.cells.griddesktop.data/gridcells/isrowhidden/)(int) | يتحقق مما إذا كان الصف في الفهرس المحدد مخفيًا. |
| [Merge](../../aspose.cells.griddesktop.data/gridcells/merge/)(int, int, int, int) | يدمج نطاقًا محددًا من الخلايا في خلية واحدة. |
| [RemoveFormulas](../../aspose.cells.griddesktop.data/gridcells/removeformulas/)() | يزيل جميع الصيغ ويستبدلها بقيمة الصيغة. |
| [SetColumnWidth](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidth/)(int, double) | يضبط عرض العمود المحدد. |
| [SetColumnWidthInch](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidthinch/)(int, double) | يضبط عرض العمود بوحدة البوصة. |
| [SetColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidthpixel/)(int, int) | يضبط عرض العمود بوحدة البكسل. |
| [SetRowHeight](../../aspose.cells.griddesktop.data/gridcells/setrowheight/)(int, double) | يضبط ارتفاع الصف المحدد. |
| [SetRowHeightInch](../../aspose.cells.griddesktop.data/gridcells/setrowheightinch/)(int, double) | يضبط ارتفاع الصف بوحدة البوصة. |
| [SetRowHeightPixel](../../aspose.cells.griddesktop.data/gridcells/setrowheightpixel/)(int, int) | يضبط ارتفاع الصف بوحدة البكسل. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle/#setstyle)(CellRange, Style) | يضبط النمط لنطاق محدد من الخلايا. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle/#setstyle_2)(string, Style) | يضبط النمط لنطاق محدد من الخلايا. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle/#setstyle_1)(int, int, int, int, Style) | يضبط النمط لنطاق محدد من الخلايا. |
| [Sort](../../aspose.cells.griddesktop.data/gridcells/sort/#sort)(int, int, int, int, int, bool, bool, bool) | يرتب البيانات تصاعديًا/تنازليًا من أعلى إلى أسفل في نطاق ورقة عمل حسب فهرس العمود المحدد. يرتب البيانات تصاعديًا/تنازليًا من اليسار إلى اليمين في نطاق ورقة عمل حسب فهرس الصف المحدد. |
| [Sort](../../aspose.cells.griddesktop.data/gridcells/sort/#sort_1)(int, int, int, int, int[], SortOrder[], SortOrientation, bool) | يرتب بيانات المنطقة. |
| [SortAsNumber](../../aspose.cells.griddesktop.data/gridcells/sortasnumber/)(int, int, int, int, int[], SortOrder[], SortOrientation) | يرتب بيانات المنطقة (يجب أن تكون بيانات العمود الرئيسي رقمًا). |
| [UngroupColumns](../../aspose.cells.griddesktop.data/gridcells/ungroupcolumns/)(int, int) | يفك تجميع الأعمدة. |
| [UngroupRows](../../aspose.cells.griddesktop.data/gridcells/ungrouprows/)(int, int) | يفك تجميع الصفوف. |
| [UnhideColumn](../../aspose.cells.griddesktop.data/gridcells/unhidecolumn/)(int, double) | يكشف عن عمود |
| [UnhideColumns](../../aspose.cells.griddesktop.data/gridcells/unhidecolumns/)(int, int, double) | يكشف عن عدة أعمدة. |
| [UnhideRow](../../aspose.cells.griddesktop.data/gridcells/unhiderow/)(int, int) | يكشف عن صف. |
| [UnhideRows](../../aspose.cells.griddesktop.data/gridcells/unhiderows/)(int, int, double) | يكشف عن الصفوف المخفية. |
| [UnMerge](../../aspose.cells.griddesktop.data/gridcells/unmerge/)(int, int, int, int) | يفك دمج نطاق محدد من الخلايا المدمجة. |
| static [CellIndexToName](../../aspose.cells.griddesktop.data/gridcells/cellindextoname/)(int, int) | يحصل على اسم الخلية وفقًا لمؤشرات الصف والعمود. |
| static [CellNameToIndex](../../aspose.cells.griddesktop.data/gridcells/cellnametoindex/)(string, out int, out int) | يحصل على فهارس الصف والعمود للخلية وفقًا لاسمها |
| static [ColumnIndexToName](../../aspose.cells.griddesktop.data/gridcells/columnindextoname/)(int) | يحصل على اسم العمود وفقًا لمؤشر العمود. |
| static [ColumnNameToIndex](../../aspose.cells.griddesktop.data/gridcells/columnnametoindex/)(string) | يحصل على مؤشر العمود وفقًا لاسم العمود. |

### انظر أيضًا

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


