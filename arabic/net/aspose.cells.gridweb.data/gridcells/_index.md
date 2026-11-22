---
title: "الفئة GridCells"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.GridWeb.Data.GridCells. تغلف مجموعة من كائنات GridCell"
type: docs
url: /ar/net/aspose.cells.gridweb.data/gridcells/
---
## GridCells class

تغلف مجموعة من كائنات [`GridCell`](../gridcell/)

```csharp
public class GridCells : IEnumerable
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Columns](../../aspose.cells.gridweb.data/gridcells/columns/) { get; } | يحصل على مجموعة كائنات [`GridColumn`](../gridcolumn/) التي تمثل الأعمدة الفردية في ورقة العمل هذه. |
| [Count](../../aspose.cells.gridweb.data/gridcells/count/) { get; } | يحصل على عدد الخلايا. |
| [FirstCell](../../aspose.cells.gridweb.data/gridcells/firstcell/) { get; } | يحصل على الخلية الأولى في ورقة العمل هذه. |
| [Item](../../aspose.cells.gridweb.data/gridcells/item/) { get; } | يحصل على العنصر [`GridCell`](../gridcell/) في فهرس صف الخلية المحدد وفهرس العمود المحدد. (مؤشرين) |
| [LastCell](../../aspose.cells.gridweb.data/gridcells/lastcell/) { get; } | يحصل على الخلية الأخيرة في ورقة العمل هذه. |
| [MaxColumn](../../aspose.cells.gridweb.data/gridcells/maxcolumn/) { get; } | الحد الأقصى لفهرس العمود للخلية التي تحتوي على بيانات أو نمط. |
| [MaxDataColumn](../../aspose.cells.gridweb.data/gridcells/maxdatacolumn/) { get; } | الحد الأقصى لفهرس العمود للخلية التي تحتوي على بيانات. |
| [MaxDataRow](../../aspose.cells.gridweb.data/gridcells/maxdatarow/) { get; } | الحد الأقصى لفهرس الصف للخلية التي تحتوي على بيانات. |
| [MaxRow](../../aspose.cells.gridweb.data/gridcells/maxrow/) { get; } | الحد الأقصى لفهرس الصف للخلية التي تحتوي على بيانات أو نمط. |
| [MergedCells](../../aspose.cells.gridweb.data/gridcells/mergedcells/) { get; } | يحصل على مجموعة الخلايا المدمجة. |
| [MinColumn](../../aspose.cells.gridweb.data/gridcells/mincolumn/) { get; } | الحد الأدنى لفهرس العمود لتلك الخلايا التي تم إنشاؤها في المجموعة (لا تشمل العمود الذي تم تعريف النمط له للعمود بأكمله ولكن لم يتم إنشاء أي خلية فيه). |
| [MinDataColumn](../../aspose.cells.gridweb.data/gridcells/mindatacolumn/) { get; } | الحد الأدنى لفهرس العمود للخلية التي تحتوي على بيانات. |
| [MinDataRow](../../aspose.cells.gridweb.data/gridcells/mindatarow/) { get; } | الحد الأدنى لمؤشر الصف للخلية التي تحتوي على بيانات. |
| [MinRow](../../aspose.cells.gridweb.data/gridcells/minrow/) { get; } | الحد الأدنى لمؤشر الصف للخلية التي تحتوي على بيانات أو نمط. |
| [RowEnumerator](../../aspose.cells.gridweb.data/gridcells/rowenumerator/) { get; } | يحصل على مُعدِّد الصفوف |
| [Rows](../../aspose.cells.gridweb.data/gridcells/rows/) { get; } | يحصل على مجموعة كائنات [`GridRow`](../gridrow/) التي تمثل الصفوف الفردية في ورقة العمل هذه. |
| [StandardHeight](../../aspose.cells.gridweb.data/gridcells/standardheight/) { get; set; } | يحصل أو يضبط ارتفاع الصف الافتراضي في ورقة العمل هذه، بوحدة النقاط. |
| [StandardHeightPixels](../../aspose.cells.gridweb.data/gridcells/standardheightpixels/) { get; set; } | يحصل أو يضبط ارتفاع الصف الافتراضي في ورقة العمل هذه، بوحدة البكسل. |
| [StandardWidth](../../aspose.cells.gridweb.data/gridcells/standardwidth/) { get; set; } | يحصل أو يضبط عرض العمود الافتراضي في ورقة العمل، بوحدة الأحرف. |
| [StandardWidthInch](../../aspose.cells.gridweb.data/gridcells/standardwidthinch/) { get; set; } | يحصل أو يعيّن عرض العمود الافتراضي في ورقة العمل، بوحدة البوصة. |
| [StandardWidthPixels](../../aspose.cells.gridweb.data/gridcells/standardwidthpixels/) { get; set; } | يحصل أو يعيّن عرض العمود الافتراضي في ورقة العمل، بوحدة البكسل. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [CheckCell](../../aspose.cells.gridweb.data/gridcells/checkcell/)(int, int) | يحصل على العنصر [`GridCell`](../gridcell/) أو null في فهرس صف الخلية المحدد وفهرس العمود المحدد. |
| [CheckColumn](../../aspose.cells.gridweb.data/gridcells/checkcolumn/)(int) | يحصل على العنصر [`GridColumn`](../gridcolumn/) أو null عند فهرس العمود المحدد. |
| [CheckRow](../../aspose.cells.gridweb.data/gridcells/checkrow/)(int) | يحصل على العنصر [`GridRow`](../gridrow/) أو null في فهرس صف الخلية المحدد. |
| [Clear](../../aspose.cells.gridweb.data/gridcells/clear/)() | امسح جميع الخلايا في المجموعة. |
| [ClearContents](../../aspose.cells.gridweb.data/gridcells/clearcontents/#clearcontents)(GridCellArea) | يمسح محتويات نطاق. |
| [ClearContents](../../aspose.cells.gridweb.data/gridcells/clearcontents/#clearcontents_1)(int, int, int, int) | يمسح محتويات نطاق. |
| [ClearFormats](../../aspose.cells.gridweb.data/gridcells/clearformats/#clearformats)(GridCellArea) | يمسح تنسيق نطاق. |
| [ClearFormats](../../aspose.cells.gridweb.data/gridcells/clearformats/#clearformats_1)(int, int, int, int) | يمسح تنسيق نطاق. |
| [ClearRange](../../aspose.cells.gridweb.data/gridcells/clearrange/#clearrange)(GridCellArea) | يمسح محتويات وتنسيق نطاق. |
| [ClearRange](../../aspose.cells.gridweb.data/gridcells/clearrange/#clearrange_1)(int, int, int, int) | يمسح محتويات وتنسيق نطاق. |
| [CopyColumn](../../aspose.cells.gridweb.data/gridcells/copycolumn/)(GridCells, int, int) | ينسخ البيانات والتنسيقات لعمود كامل. |
| [CopyColumns](../../aspose.cells.gridweb.data/gridcells/copycolumns/)(GridCells, int, int, int) | ينسخ البيانات والتنسيقات لعمود كامل. |
| [CopyRow](../../aspose.cells.gridweb.data/gridcells/copyrow/)(GridCells, int, int) | ينسخ البيانات والتنسيقات لصف كامل. |
| [CopyRows](../../aspose.cells.gridweb.data/gridcells/copyrows/)(GridCells, int, int, int) | ينسخ البيانات والتنسيقات لبعض الصفوف الكاملة. |
| [DeleteBlankColumns](../../aspose.cells.gridweb.data/gridcells/deleteblankcolumns/)() | احذف جميع الأعمدة الفارغة التي لا تحتوي على أي بيانات. |
| [DeleteBlankRows](../../aspose.cells.gridweb.data/gridcells/deleteblankrows/)() | احذف جميع الصفوف الفارغة التي لا تحتوي على أي بيانات. |
| [DeleteColumn](../../aspose.cells.gridweb.data/gridcells/deletecolumn/#deletecolumn)(int) | يحذف عمودًا. |
| [DeleteColumn](../../aspose.cells.gridweb.data/gridcells/deletecolumn/#deletecolumn_1)(int, bool) | يحذف عمودًا. |
| [DeleteColumns](../../aspose.cells.gridweb.data/gridcells/deletecolumns/)(int, int, bool) | يحذف عدة أعمدة. |
| [DeleteRange](../../aspose.cells.gridweb.data/gridcells/deleterange/)(int, int, int, int, GridShiftType) | يحذف نطاقًا من الخلايا ويُحَرِّك الخلايا وفقًا لخيار الإزاحة. |
| [DeleteRow](../../aspose.cells.gridweb.data/gridcells/deleterow/)(int) | يحذف صفًا. |
| [DeleteRows](../../aspose.cells.gridweb.data/gridcells/deleterows/#deleterows)(int, int) | يحذف عدة صفوف. |
| [DeleteRows](../../aspose.cells.gridweb.data/gridcells/deleterows/#deleterows_1)(int, int, bool) | يحذف عدة صفوف في ورقة العمل. |
| [Export](../../aspose.cells.gridweb.data/gridcells/export/)(int, int, int, int, bool, bool) | يصدّر البيانات في مجموعة Cells لعنصر WebWorksheet إلى كائن DataTable جديد |
| [ExportArray](../../aspose.cells.gridweb.data/gridcells/exportarray/)(int, int, int, int) | يصدّر البيانات في مجموعة `GridCells` إلى كائن مصفوفة ثنائية الأبعاد. |
| [GetCell](../../aspose.cells.gridweb.data/gridcells/getcell/)(int, int) | يحصل على العنصر [`GridCell`](../gridcell/) عند فهرس صف الخلية والعمود المحددين. |
| [GetColumnWidth](../../aspose.cells.gridweb.data/gridcells/getcolumnwidth/)(int) | يحصل على عرض العمود المحدد |
| [GetColumnWidthInch](../../aspose.cells.gridweb.data/gridcells/getcolumnwidthinch/)(int) | يحصل على عرض العمود المحدد، بوحدة البوصة. |
| [GetColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/getcolumnwidthpixel/)(int) | يحصل على عرض العمود المحدد، بوحدة البكسل. |
| [GetEnumerator](../../aspose.cells.gridweb.data/gridcells/getenumerator/)() | يحصل على مُعدِّد الصفوف |
| [GetRow](../../aspose.cells.gridweb.data/gridcells/getrow/)(int) | يحصل على العنصر [`GridRow`](../gridrow/) أو في فهرس صف الخلية المحدد. |
| [GetRowHeight](../../aspose.cells.gridweb.data/gridcells/getrowheight/)(int) | يحصل على ارتفاع الصف المحدد. |
| [GetRowHeightInch](../../aspose.cells.gridweb.data/gridcells/getrowheightinch/)(int) | يحصل على ارتفاع صف محدد بوحدة البوصة. |
| [GetRowHeightPixel](../../aspose.cells.gridweb.data/gridcells/getrowheightpixel/)(int) | يحصل على ارتفاع الصف المحدد بوحدة البكسل. |
| [GetRowOutlineLevel](../../aspose.cells.gridweb.data/gridcells/getrowoutlinelevel/)(int) | يحصل على مستوى المخطط للصف. |
| [GetViewColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/getviewcolumnwidthpixel/)(int) | احصل على العرض في نوع عرض مختلف. |
| [GroupColumns](../../aspose.cells.gridweb.data/gridcells/groupcolumns/#groupcolumns)(int, int) | يقوم بتجميع الأعمدة. |
| [GroupColumns](../../aspose.cells.gridweb.data/gridcells/groupcolumns/#groupcolumns_1)(int, int, bool) | يقوم بتجميع الأعمدة. |
| [GroupRows](../../aspose.cells.gridweb.data/gridcells/grouprows/)(int, int) | يقوم بتجميع الصفوف. |
| [HideColumn](../../aspose.cells.gridweb.data/gridcells/hidecolumn/)(int) | يخفي عمودًا. |
| [HideRow](../../aspose.cells.gridweb.data/gridcells/hiderow/)(int) | يخفي صفًا. |
| [InsertColumn](../../aspose.cells.gridweb.data/gridcells/insertcolumn/#insertcolumn)(int) | يدرج عمودًا جديدًا في ورقة العمل. |
| [InsertColumn](../../aspose.cells.gridweb.data/gridcells/insertcolumn/#insertcolumn_1)(int, bool) | يدرج عمودًا جديدًا في ورقة العمل. |
| [InsertColumns](../../aspose.cells.gridweb.data/gridcells/insertcolumns/#insertcolumns)(int, int) | يدرج بعض الأعمدة في ورقة العمل. |
| [InsertColumns](../../aspose.cells.gridweb.data/gridcells/insertcolumns/#insertcolumns_1)(int, int, bool) | يدرج بعض الأعمدة في ورقة العمل. |
| [InsertRange](../../aspose.cells.gridweb.data/gridcells/insertrange/#insertrange)(GridCellArea, GridShiftType) | يدرج نطاقًا من الخلايا ويُحرك الخلايا وفقًا لخيار التحريك. |
| [InsertRange](../../aspose.cells.gridweb.data/gridcells/insertrange/#insertrange_1)(GridCellArea, int, GridShiftType, bool) | يدرج نطاقًا من الخلايا ويُحرك الخلايا وفقًا لخيار التحريك. |
| [InsertRow](../../aspose.cells.gridweb.data/gridcells/insertrow/)(int) | يدرج صفًا جديدًا في ورقة العمل. |
| [InsertRows](../../aspose.cells.gridweb.data/gridcells/insertrows/#insertrows)(int, int) | يدرج عدة صفوف في ورقة العمل. |
| [InsertRows](../../aspose.cells.gridweb.data/gridcells/insertrows/#insertrows_1)(int, int, bool) | يدرج عدة صفوف في ورقة العمل. |
| [IsBlankColumn](../../aspose.cells.gridweb.data/gridcells/isblankcolumn/)(int) | يتحقق مما إذا كان العمود المحدد فارغًا (لا يحتوي على أي بيانات). |
| [IsColumnHidden](../../aspose.cells.gridweb.data/gridcells/iscolumnhidden/)(int) | يتحقق مما إذا كان العمود في الفهرس المحدد مخفيًا. |
| [IsRowHidden](../../aspose.cells.gridweb.data/gridcells/isrowhidden/)(int) | يتحقق مما إذا كان الصف في الفهرس المحدد مخفيًا. |
| [Merge](../../aspose.cells.gridweb.data/gridcells/merge/)(int, int, int, int) | يدمج نطاقًا محددًا من الخلايا في خلية واحدة. |
| [MoveRange](../../aspose.cells.gridweb.data/gridcells/moverange/)(GridCellArea, int, int) | ينقل النطاق. |
| [RemoveDuplicates](../../aspose.cells.gridweb.data/gridcells/removeduplicates/)(int, int, int, int) | إزالة القيم المكررة في النطاق. |
| [RemoveFormulas](../../aspose.cells.gridweb.data/gridcells/removeformulas/)() | يزيل جميع الصيغ ويستبدلها بقيمة الصيغة. |
| [SetBorders](../../aspose.cells.gridweb.data/gridcells/setborders/)(int, int, int, int, SetBorderPosition, WebBorderStyle) | يضبط الحدود لنطاق خلايا. |
| [SetColumnWidth](../../aspose.cells.gridweb.data/gridcells/setcolumnwidth/)(int, double) | يضبط عرض العمود المحدد. |
| [SetColumnWidthInch](../../aspose.cells.gridweb.data/gridcells/setcolumnwidthinch/)(int, double) | يضبط عرض العمود بوحدة البوصة. |
| [SetColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/setcolumnwidthpixel/)(int, int) | يضبط عرض العمود بوحدة البكسل. |
| [SetRowHeight](../../aspose.cells.gridweb.data/gridcells/setrowheight/)(int, double) | يضبط ارتفاع الصف المحدد. |
| [SetRowHeightInch](../../aspose.cells.gridweb.data/gridcells/setrowheightinch/)(int, double) | يضبط ارتفاع الصف بوحدة البوصة. |
| [SetRowHeightPixel](../../aspose.cells.gridweb.data/gridcells/setrowheightpixel/)(int, int) | يضبط ارتفاع الصف بوحدة البكسل. |
| [SetRowOutlineLevel](../../aspose.cells.gridweb.data/gridcells/setrowoutlinelevel/)(int, int) | يضبط مستوى المخطط للصف. |
| [SetStyle](../../aspose.cells.gridweb.data/gridcells/setstyle/#setstyle_1)(string, GridTableItemStyle) | يضبط النمط لنطاق محدد من الخلايا. |
| [SetStyle](../../aspose.cells.gridweb.data/gridcells/setstyle/#setstyle)(int, int, int, int, GridTableItemStyle) | يضبط النمط لنطاق محدد من الخلايا. |
| [Sort](../../aspose.cells.gridweb.data/gridcells/sort/#sort)(int, int, int, int, int, bool, bool, bool) | يرتب البيانات تصاعديًا/تنازليًا من أعلى إلى أسفل في نطاق ورقة عمل حسب فهرس العمود المحدد. يرتب البيانات تصاعديًا/تنازليًا من اليسار إلى اليمين في نطاق ورقة عمل حسب فهرس الصف المحدد. |
| [Sort](../../aspose.cells.gridweb.data/gridcells/sort/#sort_1)(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) | يرتب البيانات تصاعديًا/تنازليًا من أعلى إلى أسفل في نطاق ورقة عمل حسب فهرس العمود المحدد. يرتب البيانات تصاعديًا/تنازليًا من اليسار إلى اليمين في نطاق ورقة عمل حسب فهرس الصف المحدد. |
| [UngroupColumns](../../aspose.cells.gridweb.data/gridcells/ungroupcolumns/)(int, int) | يفك تجميع الأعمدة. |
| [UngroupRows](../../aspose.cells.gridweb.data/gridcells/ungrouprows/)(int, int) | يفك تجميع الصفوف. |
| [UnhideColumn](../../aspose.cells.gridweb.data/gridcells/unhidecolumn/)(int, double) | يكشف عن عمود |
| [UnhideRow](../../aspose.cells.gridweb.data/gridcells/unhiderow/)(int) | يكشف عن صف. |
| [UnMerge](../../aspose.cells.gridweb.data/gridcells/unmerge/)(int, int, int, int) | يفك دمج نطاق محدد من الخلايا المدمجة. |
| static [CellIndexToName](../../aspose.cells.gridweb.data/gridcells/cellindextoname/)(int, int) | يحصل على اسم الخلية وفقًا لمؤشرات الصف والعمود. |
| static [CellNameToIndex](../../aspose.cells.gridweb.data/gridcells/cellnametoindex/)(string, out int, out int) | يحصل على فهارس الصف والعمود للخلية وفقًا لاسمها |
| static [ColumnIndexToName](../../aspose.cells.gridweb.data/gridcells/columnindextoname/)(int) | يحصل على اسم العمود وفقًا لمؤشر العمود. |
| static [ColumnNameToIndex](../../aspose.cells.gridweb.data/gridcells/columnnametoindex/)(string) | يحصل على مؤشر العمود وفقًا لاسم العمود. |

### انظر أيضًا

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


