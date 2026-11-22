---
title: "الفئة WebCells"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.GridWeb.Data.WebCells class."
type: docs
url: /ar/net/aspose.cells.gridweb.data/webcells/
---
## WebCells class

```csharp
[Obsolete("This class is obsolete; use  GridCells instead")]
public class WebCells
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/webcells/count/) { get; } | يحصل على عدد الخلايا. |
| [Item](../../aspose.cells.gridweb.data/webcells/item/) { get; } | يحصل على عنصر الخلية عند فهرس صف الخلية المحدد وفهرس العمود المحدد. (مؤشرين) |
| [MaxColumn](../../aspose.cells.gridweb.data/webcells/maxcolumn/) { get; } |  |
| [MaxRow](../../aspose.cells.gridweb.data/webcells/maxrow/) { get; } |  |
| [MergedCells](../../aspose.cells.gridweb.data/webcells/mergedcells/) { get; } | يحصل على مجموعة الخلايا المدمجة. |
| [MinColumn](../../aspose.cells.gridweb.data/webcells/mincolumn/) { get; } | الحد الأدنى لرقم العمود للخلية التي تحتوي على بيانات أو نمط. |
| [MinRow](../../aspose.cells.gridweb.data/webcells/minrow/) { get; } | الحد الأدنى لرقم الصف للخلية التي تحتوي على بيانات أو نمط. |
| [StandardHeight](../../aspose.cells.gridweb.data/webcells/standardheight/) { get; set; } | يحصل أو يضبط ارتفاع الصف الافتراضي في ورقة العمل هذه، بوحدة النقاط. |
| [StandardWidth](../../aspose.cells.gridweb.data/webcells/standardwidth/) { get; set; } | يحصل أو يضبط عرض العمود الافتراضي في ورقة العمل، بوحدة الأحرف. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Clear](../../aspose.cells.gridweb.data/webcells/clear/)() |  |
| [ClearContents](../../aspose.cells.gridweb.data/webcells/clearcontents/)(int, int, int, int) | يمسح محتويات نطاق. |
| [DeleteColumn](../../aspose.cells.gridweb.data/webcells/deletecolumn/)(int) | يحذف عمودًا. |
| [DeleteRow](../../aspose.cells.gridweb.data/webcells/deleterow/)(int) | يحذف صفًا. |
| [DeleteRows](../../aspose.cells.gridweb.data/webcells/deleterows/)(int, int) | يحذف عددًا من الصفوف. هذه الطريقة أسرع بكثير من DeleteRow عند حذف صفوف دفعة واحدة. |
| [Export](../../aspose.cells.gridweb.data/webcells/export/)(int, int, int, int, bool, bool) | يصدّر البيانات في مجموعة Cells لعنصر WebWorksheet إلى كائن DataTable جديد |
| [ExportArray](../../aspose.cells.gridweb.data/webcells/exportarray/)(int, int, int, int) | يصدّر البيانات في مجموعة Cells إلى كائن مصفوفة ثنائية الأبعاد. |
| [GetColumnCaption](../../aspose.cells.gridweb.data/webcells/getcolumncaption/)(int) | يحصل على تسمية العمود. إذا لم يتم تعيين التسمية، يرجع سلسلة فارغة. |
| [GetColumnReadonly](../../aspose.cells.gridweb.data/webcells/getcolumnreadonly/)(int) | يحصل على ما إذا كان العمود للقراءة فقط. هذه طريقة موسعة من GridWeb تحديدًا، لن تُحفظ أو تُؤثر في ملف Excel الفعلي. |
| [GetColumnWidth](../../aspose.cells.gridweb.data/webcells/getcolumnwidth/)(int) | يحصل على عرض العمود المحدد |
| [GetEnumerator](../../aspose.cells.gridweb.data/webcells/getenumerator/)() | يسترجع عداد الخلايا |
| [GetRowCaption](../../aspose.cells.gridweb.data/webcells/getrowcaption/)(int) | يحصل على تسمية الصف. إذا لم يتم تعيين التسمية، يرجع سلسلة فارغة. |
| [GetRowHeight](../../aspose.cells.gridweb.data/webcells/getrowheight/)(int) | يحصل على ارتفاع الصف المحدد. |
| [GetRowHiddenStatus](../../aspose.cells.gridweb.data/webcells/getrowhiddenstatus/)(int) | احصل على حالة الإخفاء لصف محدد. |
| [GetRowOutlineLevel](../../aspose.cells.gridweb.data/webcells/getrowoutlinelevel/)(int) | يحصل على مستوى المخطط للصف. |
| [GetRowReadonly](../../aspose.cells.gridweb.data/webcells/getrowreadonly/)(int) | يحصل على ما إذا كان الصف للقراءة فقط. هذه طريقة موسعة من GridWeb تحديدًا، لن تُحفظ ولن تؤثر في ملف Excel الفعلي. |
| [InsertColumn](../../aspose.cells.gridweb.data/webcells/insertcolumn/)(int) | يدرج عمودًا جديدًا في ورقة العمل. |
| [InsertRow](../../aspose.cells.gridweb.data/webcells/insertrow/)(int) | يدرج صفًا جديدًا في ورقة العمل. |
| [InsertRows](../../aspose.cells.gridweb.data/webcells/insertrows/)(int, int) | يدرج عدة صفوف في ورقة العمل. |
| [Merge](../../aspose.cells.gridweb.data/webcells/merge/)(int, int, int, int) |  |
| [SetBorders](../../aspose.cells.gridweb.data/webcells/setborders/)(int, int, int, int, SetBorderPosition, WebBorderStyle) | يضبط الحدود لنطاق خلايا. |
| [SetColumnCaption](../../aspose.cells.gridweb.data/webcells/setcolumncaption/)(int, string) | يضبط التسمية للعمود. يرجى ملاحظة أن هذه سمة امتداد ولا يمكن حفظها في ملف Excel. |
| [SetColumnReadonly](../../aspose.cells.gridweb.data/webcells/setcolumnreadonly/)(int, bool) | يضبط عمودًا للقراءة فقط بحيث لا يستطيع المستخدم حذفه من جانب العميل. هذه طريقة موسعة من GridWeb تحديدًا، لن تُحفظ ولن تؤثر في ملف Excel الفعلي. |
| [SetColumnWidth](../../aspose.cells.gridweb.data/webcells/setcolumnwidth/)(int, Unit) | يحدد عرض العمود المحدد. نوع العرض المقبول هو Point,Pixel أو Inch |
| [SetRowCaption](../../aspose.cells.gridweb.data/webcells/setrowcaption/)(int, string) | يضبط التسمية للصف. |
| [SetRowHeight](../../aspose.cells.gridweb.data/webcells/setrowheight/)(int, Unit) | يحدد ارتفاع الصف المحدد. نوع العرض المقبول هو Point,Pixel أو Inch |
| [SetRowHiddenStatus](../../aspose.cells.gridweb.data/webcells/setrowhiddenstatus/)(int, bool) | حدد حالة الإخفاء لصف محدد. |
| [SetRowOutlineLevel](../../aspose.cells.gridweb.data/webcells/setrowoutlinelevel/)(int, int) | يضبط مستوى المخطط للصف. |
| [SetRowOutlineLevelAndStatus](../../aspose.cells.gridweb.data/webcells/setrowoutlinelevelandstatus/)(int, int, bool) | يضبط مستوى المخطط للصف. |
| [SetRowReadonly](../../aspose.cells.gridweb.data/webcells/setrowreadonly/)(int, bool) | يضبط صفًا للقراءة فقط بحيث لا يستطيع المستخدم حذفه من جانب العميل. هذه طريقة موسعة من GridWeb تحديدًا، لن تُحفظ ولن تؤثر في ملف Excel الفعلي. |
| [SetStyle](../../aspose.cells.gridweb.data/webcells/setstyle/#setstyle_1)(string, TableItemStyle) | يضبط النمط لنطاق محدد من الخلايا. |
| [SetStyle](../../aspose.cells.gridweb.data/webcells/setstyle/#setstyle)(int, int, int, int, TableItemStyle) | يضبط النمط لنطاق محدد من الخلايا. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort)(int, int, int, int, int) | يرتب البيانات تصاعديًا من الأعلى إلى الأسفل في نطاق WebWorksheet حسب فهرس العمود المحدد. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_2)(int, int, int, int, int[]) | يرتب البيانات تصاعديًا من الأعلى إلى الأسفل في نطاق WebWorksheet حسب بعض الحقول المحددة بواسطة مصفوفة فهارس الأعمدة. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_1)(int, int, int, int, int, SortByOrder, SortOrientation, bool) | يرتب البيانات تصاعديًا من الأعلى إلى الأسفل في نطاق WebWorksheet حسب فهرس العمود المحدد. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_3)(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) | يرتب البيانات تصاعديًا في نطاق WebWorksheet حسب بعض الحقول المحددة بواسطة مصفوفة الفهارس. |
| [UnMerge](../../aspose.cells.gridweb.data/webcells/unmerge/)(int, int, int, int) | يفك دمج نطاق محدد من الخلايا المدمجة. |
| static [CellIndexToName](../../aspose.cells.gridweb.data/webcells/cellindextoname/)(int, int) | يحصل على اسم الخلية وفقًا لمؤشرات الصف والعمود. |
| static [CellNameToIndex](../../aspose.cells.gridweb.data/webcells/cellnametoindex/)(string, out int, out int) | يحصل على فهارس الصف والعمود للخلية وفقًا لاسمها |
| static [ColumnIndexToName](../../aspose.cells.gridweb.data/webcells/columnindextoname/)(int) | يحصل على اسم العمود وفقًا لمؤشر العمود. |
| static [ColumnNameToIndex](../../aspose.cells.gridweb.data/webcells/columnnametoindex/)(string) | يحصل على مؤشر العمود وفقًا لاسم العمود. |

### ملاحظات

ملاحظة: هذه الفئة أصبحت الآن مهجورة. يرجى استخدام GridCells بدلاً من ذلك. سيتم إزالة هذه الفئة بعد 6 أشهر من أغسطس 2014. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### انظر أيضًا

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


