---
title: ColumnCollection
second_title: Aspose.Cells لمرجع .NET API
description: مجموعة منالكائنات التي تمثل الأعمدة الفردية الإعدادات في ورقة العمل . يمثل كائن العمود فقط الإعدادات مثل عرض العمود والأنماط وما إلى ذلك. بالنسبة للعمود بأكمله  لا علاقة له بحقيقة وجود خلايا بيانات غير فارغة أو ليست في العمود المقابل. المجموعة  لا علاقة لها بحقيقة وجود خلايا غير فارغة بيانات أو لا توجد في ورقة العمل.
type: docs
weight: 1070
url: /ar/net/aspose.cells/columncollection/
---
## ColumnCollection class

مجموعة منالكائنات التي تمثل الأعمدة الفردية (الإعدادات) في ورقة العمل . يمثل كائن العمود فقط الإعدادات مثل عرض العمود والأنماط وما إلى ذلك. بالنسبة للعمود بأكمله ، لا علاقة له بحقيقة وجود خلايا (بيانات) غير فارغة أو ليست في العمود المقابل. المجموعة ، لا علاقة لها بحقيقة وجود خلايا غير فارغة (بيانات) أو لا توجد في ورقة العمل.

```csharp
public class ColumnCollection : CollectionBase<Column>
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells/columncollection/item) { get; } | يحصل على أ كائن حسب فهرس العمود . سيتم إنشاء مثيل كائن العمود الخاص بفهرس العمود المحدد إذا لم يكن موجودًا من قبل. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## طُرق

| اسم | وصف |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Column) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Column, IComparer&lt;Column&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Column, IComparer&lt;Column&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Column) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Column[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Column[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Column[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Column&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Column&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Column&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Column&gt;) |  |
| [GetColumnByIndex](../../aspose.cells/columncollection/getcolumnbyindex)(int) | يحصل على ملف[`Column`](../column)الكائن بالموقع في القائمة . |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Column) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Column, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Column, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Column) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Column, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Column, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### أمثلة

```csharp

[C#]

// إنشاء كائن مصنف
Workbook workbook = new Workbook();

// الحصول على مرجع ورقة العمل الأولى
Worksheet worksheet = workbook.Worksheets[0];

// إضافة نمط جديد إلى المصنف
Style style = workbook.CreateStyle();

// ضبط لون الخلفية على اللون الأزرق
style.ForegroundColor = Color.Blue;

// إعداد نمط الخلفية
style.Pattern = BackgroundType.Solid;

// علم نمط جديد
StyleFlag styleFlag = new StyleFlag();

// تعيين كافة الأنماط
styleFlag.All = true;

// تغيير العرض الافتراضي للأعمدة العشرة الأولى
for (int i = 0; i < 10; i++)
{
    worksheet.Cells.Columns[i].Width = 20;
}

// احصل على العمود بتنسيق غير افتراضي
ColumnCollection columns = worksheet.Cells.Columns;

foreach (Column column in columns)
{
    // تطبيق النمط على الأعمدة العشرة الأولى
    column.ApplyStyle(style, styleFlag);
}

// حفظ ملف Excel
workbook.Save("book1.xls");

[VB.NET]

'إنشاء كائن مصنف
Dim workbook As Workbook = New Workbook()

'الحصول على مرجع ورقة العمل الأولى
Dim worksheet As Worksheet = workbook.Worksheets(0)

'إضافة نمط جديد إلى المصنف
Dim style As Style = workbook.CreateStyles()

'ضبط لون الخلفية على اللون الأزرق
style.ForegroundColor = Color.Blue

'ضبط نمط الخلفية
style.Pattern = BackgroundType.Solid

'علم نمط جديد
Dim styleFlag As New StyleFlag()

'تعيين كافة الأنماط
styleFlag.All = True

'قم بتغيير العرض الافتراضي للأعمدة العشرة الأولى
For i As Integer = 0 To 9
    worksheet.Cells.Columns(i).Width = 20
Next i

'احصل على العمود بتنسيق غير افتراضي
Dim columns As ColumnCollection = worksheet.Cells.Columns

For Each column As Column In columns
    'قم بتطبيق النمط على الأعمدة العشرة الأولى
    column.ApplyStyle(style, styleFlag)
Next column

'حفظ ملف Excel
workbook.Save("book1.xls")

```

### أنظر أيضا

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [Column](../column)
* مساحة الاسم [Aspose.Cells](../../aspose.cells)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
