---
title: ListObject
second_title: Aspose.Cells لمرجع .NET API
description: يمثل كائن قائمة في ورقة عمل . كائن ListObject هو عضو في مجموعة ListObjects. تحتوي مجموعة ListObjects على كافة كائنات القائمة في ورقة العمل.
type: docs
weight: 5820
url: /ar/net/aspose.cells.tables/listobject/
---
## ListObject class

يمثل كائن قائمة في ورقة عمل . كائن ListObject هو عضو في مجموعة ListObjects. تحتوي مجموعة ListObjects على كافة كائنات القائمة في ورقة العمل.

```csharp
public class ListObject
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [AlternativeDescription](../../aspose.cells.tables/listobject/alternativedescription) { get; set; } | الحصول على الوصف البديل وتعيينه. |
| [AlternativeText](../../aspose.cells.tables/listobject/alternativetext) { get; set; } | الحصول على النص البديل وتعيينه. |
| [AutoFilter](../../aspose.cells.tables/listobject/autofilter) { get; } | يحصل على مرشح تلقائي . |
| [Comment](../../aspose.cells.tables/listobject/comment) { get; set; } | الحصول على تعليق الجدول وتعيينه. |
| [DataRange](../../aspose.cells.tables/listobject/datarange) { get; } | الحصول على نطاق بيانات ListObject . |
| [DataSourceType](../../aspose.cells.tables/listobject/datasourcetype) { get; } | يحصل على نوع مصدر البيانات الخاص بالجدول. |
| [DisplayName](../../aspose.cells.tables/listobject/displayname) { get; set; } | الحصول على اسم العرض وتعيينه. |
| [EndColumn](../../aspose.cells.tables/listobject/endcolumn) { get; } | يحصل على عمود نهاية النطاق . |
| [EndRow](../../aspose.cells.tables/listobject/endrow) { get; } | يحصل على صف نهاية النطاق . |
| [ListColumns](../../aspose.cells.tables/listobject/listcolumns) { get; } | الحصول على قائمةأعمدة ListObject. |
| [QueryTable](../../aspose.cells.tables/listobject/querytable) { get; } | يحصل على جدول الاستعلام المرتبط . |
| [ShowHeaderRow](../../aspose.cells.tables/listobject/showheaderrow) { get; set; } | يحصل ويعين ما إذا كانت ListObject هذه تعرض صف الرأس. |
| [ShowTableStyleColumnStripes](../../aspose.cells.tables/listobject/showtablestylecolumnstripes) { get; set; } | يشير إلى ما إذا كان تنسيق شريط العمود مطبقًا . |
| [ShowTableStyleFirstColumn](../../aspose.cells.tables/listobject/showtablestylefirstcolumn) { get; set; } | يشير إلى ما إذا كان يجب تطبيق النمط المطبق على العمود الأول في الجدول. |
| [ShowTableStyleLastColumn](../../aspose.cells.tables/listobject/showtablestylelastcolumn) { get; set; } | يشير إلى ما إذا كان يجب تطبيق النمط المطبق على العمود الأخير في الجدول. |
| [ShowTableStyleRowStripes](../../aspose.cells.tables/listobject/showtablestylerowstripes) { get; set; } | يشير إلى ما إذا كان يتم تطبيق تنسيق شريط الصف. |
| [ShowTotals](../../aspose.cells.tables/listobject/showtotals) { get; set; } | يحصل ويعين ما إذا كان كائن ListObject هذا يعرض الصف الإجمالي. |
| [StartColumn](../../aspose.cells.tables/listobject/startcolumn) { get; } | يحصل على عمود البداية للنطاق . |
| [StartRow](../../aspose.cells.tables/listobject/startrow) { get; } | يحصل على صف بداية النطاق . |
| [TableStyleName](../../aspose.cells.tables/listobject/tablestylename) { get; set; } | الحصول على اسم نمط الجدول وتعيينه. |
| [TableStyleType](../../aspose.cells.tables/listobject/tablestyletype) { get; set; } | يحصل ونمط الجدول المدمج . |
| [XmlMap](../../aspose.cells.tables/listobject/xmlmap) { get; } | يحصل على ملف[`XmlMap`](./xmlmap)المستخدمة لهذه القائمة. |

## طُرق

| اسم | وصف |
| --- | --- |
| [ApplyStyleToRange](../../aspose.cells.tables/listobject/applystyletorange)() | قم بتطبيق نمط الجدول على النطاق . |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange#converttorange)() | تحويل الجدول إلى النطاق . |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange#converttorange_1)(TableToRangeOptions) | تحويل الجدول إلى النطاق . |
| [Filter](../../aspose.cells.tables/listobject/filter)() | تصفية الجدول . |
| [PutCellValue](../../aspose.cells.tables/listobject/putcellvalue)(int, int, object) | ضع القيمة في الخلية. |
| [Resize](../../aspose.cells.tables/listobject/resize)(int, int, int, int, bool) | تغيير حجم نطاق كائن القائمة . |
| [UpdateColumnName](../../aspose.cells.tables/listobject/updatecolumnname)() | يقوم بتحديث جميع أسماء أعمدة القائمة من ورقة العمل. |

### أمثلة

```csharp

[C#]


Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
for (int i = 0; i  <5; i++)
{
cells[0,i].PutValue(CellsHelper.ColumnIndexToName(i));
 }
for (int row = 1; row  <10; row++)
{
 for (int column = 0; column  <5; column++)
{
cells[row, column].PutValue(row * column);
 }
 }
ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
int index = tables.Add(0, 0, 9, 4, true);
ListObject table = tables[0];
table.ShowTotals = true;
table.ListColumns[4].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;
workbook.Save(@"Book1.xlsx");


[Visual Basic]

Dim workbook As Workbook = New Workbook()
Dim cells As Cells = workbook.Worksheets(0).Cells
For i As Int32 = 0 To 4
 cells(0, i).PutValue(CellsHelper.ColumnIndexToName(i))
Next
For row As Int32 = 1 To 9
 For column As Int32 = 0 To 4
  cells(row, column).PutValue(row * column)
Next
Next
Dim tables As ListObjectCollection = workbook.Worksheets(0).ListObjects
Dim index As Int32 = tables.Add(0, 0, 9, 4, True)
Dim table As ListObject = tables(0)
table.ShowTotals = True
table.ListColumns(4).TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum
workbook.Save("Book1.xlsx")
```

### أنظر أيضا

* مساحة الاسم [Aspose.Cells.Tables](../../aspose.cells.tables)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
