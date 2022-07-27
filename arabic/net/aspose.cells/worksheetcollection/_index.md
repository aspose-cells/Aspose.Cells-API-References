---
title: WorksheetCollection
second_title: Aspose.Cells لمرجع .NET API
description: لتغليف مجموعة منWorksheet./worksheet الكائنات .
type: docs
weight: 6520
url: /ar/net/aspose.cells/worksheetcollection/
---
## WorksheetCollection class

لتغليف مجموعة من[`Worksheet`](../worksheet) الكائنات .

```csharp
public class WorksheetCollection : CollectionBase<Worksheet>
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells/worksheetcollection/activesheetindex) { get; set; } | يمثل فهرس ورقة العمل النشطة عند فتح جدول البيانات. |
| [ActiveSheetName](../../aspose.cells/worksheetcollection/activesheetname) { get; set; } | يمثل اسم ورقة العمل النشطة عند فتح جدول البيانات. |
| [BuiltInDocumentProperties](../../aspose.cells/worksheetcollection/builtindocumentproperties) { get; } | إرجاع أ[`DocumentProperty`](../../aspose.cells.properties/documentproperty)مجموعة تمثل جميع خصائص المستند المضمنة في جدول البيانات. |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [CustomDocumentProperties](../../aspose.cells/worksheetcollection/customdocumentproperties) { get; } | إرجاع أ[`DocumentProperty`](../../aspose.cells.properties/documentproperty) المجموعة التي تمثل جميع خصائص المستند المخصصة لجدول البيانات. |
| [Dxfs](../../aspose.cells/worksheetcollection/dxfs) { get; } | يحصل على سجلات التنسيق التفاضلي الرئيسية. |
| [ExternalLinks](../../aspose.cells/worksheetcollection/externallinks) { get; } | يمثل ارتباطات خارجية في مصنف. |
| [IsRefreshAllConnections](../../aspose.cells/worksheetcollection/isrefreshallconnections) { get; set; } | يشير إلى ما إذا كان يتم تحديث كافة الاتصالات عند فتح ملف في MS Excel. |
| [Item](../../aspose.cells/worksheetcollection/item) { get; } | يحصل على ملف[`Worksheet`](../worksheet) عنصر في الفهرس المحدد. (2 indexers) |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |
| [Names](../../aspose.cells/worksheetcollection/names) { get; } | الحصول على مجموعة كل كائنات الاسم في جدول البيانات. |
| [OleSize](../../aspose.cells/worksheetcollection/olesize) { get; set; } | الحصول على الحجم المعروض وتعيينه عند استخدام ملف المصنف ككائن Ole. |
| [RevisionLogs](../../aspose.cells/worksheetcollection/revisionlogs) { get; } | يمثل سجلات المراجعة. |
| [TableStyles](../../aspose.cells/worksheetcollection/tablestyles) { get; } | يحصل[`TableStyles`](./tablestyles) الكائن . |
| [ThreadedCommentAuthors](../../aspose.cells/worksheetcollection/threadedcommentauthors) { get; } | الحصول على قائمة مؤلفي التعليقات المترابطة. |
| [WebExtensions](../../aspose.cells/worksheetcollection/webextensions) { get; } | الحصول على قائمة أجزاء المهام. |
| [WebExtensionTaskPanes](../../aspose.cells/worksheetcollection/webextensiontaskpanes) { get; } | الحصول على قائمة أجزاء المهام. |
| [XmlMaps](../../aspose.cells/worksheetcollection/xmlmaps) { get; set; } | الحصول على خرائط XML وتعيينها في المصنف. |

## طُرق

| اسم | وصف |
| --- | --- |
| [Add](../../aspose.cells/worksheetcollection/add#add_1)() | يضيف ورقة عمل إلى المجموعة. |
| [Add](../../aspose.cells/worksheetcollection/add#add_2)(SheetType) | يضيف ورقة عمل إلى المجموعة. |
| [Add](../../aspose.cells/worksheetcollection/add#add)(string) | يضيف ورقة عمل إلى المجموعة. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy#addcopy)(int) | إضافة ورقة عمل إلى المجموعة ونسخ البيانات من ورقة عمل موجودة. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy#addcopy_1)(string) | إضافة ورقة عمل إلى المجموعة ونسخ البيانات من ورقة عمل موجودة. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Worksheet) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [Clear](../../aspose.cells/worksheetcollection/clear#clear)() | مسح كافة أوراق العمل. (2 methods) |
| [ClearPivottables](../../aspose.cells/worksheetcollection/clearpivottables)() | مسح الجداول المحورية من جدول البيانات. |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Worksheet) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Worksheet[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Worksheet[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Worksheet[], int, int) |  |
| [CreateRange](../../aspose.cells/worksheetcollection/createrange)(string, int) | ينشئ ملف[`Range`](../range) كائن من عنوان النطاق . |
| [CreateUnionRange](../../aspose.cells/worksheetcollection/createunionrange)(string, int) | ينشئ ملف[`Range`](../range) كائن من عنوان النطاق . |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Worksheet&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Worksheet&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [GetNamedRanges](../../aspose.cells/worksheetcollection/getnamedranges)() | يحصل على جميع النطاقات المحددة مسبقًا في جدول البيانات. |
| [GetNamedRangesAndTables](../../aspose.cells/worksheetcollection/getnamedrangesandtables)() | يحصل على جميع النطاقات المحددة مسبقًا في جدول البيانات. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname#getrangebyname)(string) | يحصل على كائن النطاق باسم محدد مسبقًا. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname#getrangebyname_1)(string, int, bool) | يحصل[`Range`](../range) حسب الاسم المحدد مسبقًا أو اسم الجدول |
| [GetSheetByCodeName](../../aspose.cells/worksheetcollection/getsheetbycodename)(string) | يحصل على ورقة العمل بالاسم الرمزي. |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet, int, int) |  |
| [Insert](../../aspose.cells/worksheetcollection/insert#insert)(int, SheetType) | أدخل ورقة عمل . |
| [Insert](../../aspose.cells/worksheetcollection/insert#insert_1)(int, SheetType, string) | أدخل ورقة عمل . |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet, int, int) |  |
| [RefreshPivotTables](../../aspose.cells/worksheetcollection/refreshpivottables)() | يقوم بتحديث كافة جداول PivotTables الموجودة في مجموعة أوراق العمل. |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction#registeraddinfunction_1)(int, string) | يضيف وظيفة الوظيفة الإضافية في المصنف |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction#registeraddinfunction)(string, string, bool) | يضيف وظيفة الوظيفة الإضافية في المصنف |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat#removeat)(int) | يزيل العنصر في فهرس محدد . (2 methods) |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat#removeat_2)(string) | يزيل العنصر باسم محدد . |
| [SetOleSize](../../aspose.cells/worksheetcollection/setolesize)(int, int, int, int) | يضبط الحجم المعروض عند استخدام ملف المصنف ككائن Ole. |
| [SortNames](../../aspose.cells/worksheetcollection/sortnames)() | يقوم بفرز الأسماء المعرفة . |
| [SwapSheet](../../aspose.cells/worksheetcollection/swapsheet)(int, int) | تبديل الورقتين . |

### أمثلة

```csharp
[C#]

Workbook workbook = new Workbook();

WorksheetCollection sheets = workbook.Worksheets;

// أضف ورقة عمل
sheets.Add();

// تغيير اسم ورقة العمل
sheets[0].Name = "First Sheet";

// اضبط الورقة النشطة على ورقة العمل الثانية
sheets.ActiveSheetIndex = 1;

	
[Visual Basic]

Dim excel as Workbook = new Workbook()

Dim sheets as WorksheetCollection = excel.Worksheets

'أضف ورقة عمل
sheets.Add()

'قم بتغيير اسم ورقة العمل
sheets(0).Name = "First Sheet"

'اضبط الورقة النشطة على ورقة العمل الثانية
sheets.ActiveSheetIndex = 1
```

### أنظر أيضا

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [Worksheet](../worksheet)
* مساحة الاسم [Aspose.Cells](../../aspose.cells)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
