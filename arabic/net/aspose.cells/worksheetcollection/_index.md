---
title: "الفئة WorksheetCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.WorksheetCollection. تغلف مجموعة من كائنات Worksheet"
type: docs
url: /ar/net/aspose.cells/worksheetcollection/
---
## WorksheetCollection class

تغلف مجموعة من كائنات [`Worksheet`](../worksheet/).

```csharp
public class WorksheetCollection : CollectionBase<Worksheet>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells/worksheetcollection/activesheetindex/) { get; set; } | يمثل فهرس ورقة العمل النشطة عند فتح جدول البيانات. |
| [ActiveSheetName](../../aspose.cells/worksheetcollection/activesheetname/) { get; set; } | يمثل اسم ورقة العمل النشطة عند فتح جدول البيانات. |
| [BuiltInDocumentProperties](../../aspose.cells/worksheetcollection/builtindocumentproperties/) { get; } | يعيد مجموعة [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) التي تمثل جميع خصائص المستند المدمجة في جدول البيانات. |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [CustomDocumentProperties](../../aspose.cells/worksheetcollection/customdocumentproperties/) { get; } | يعيد مجموعة [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) التي تمثل جميع خصائص المستند المخصصة في جدول البيانات. |
| [Dxfs](../../aspose.cells/worksheetcollection/dxfs/) { get; } | يحصل على سجلات تنسيق الفروقات الرئيسية. |
| [ExternalLinks](../../aspose.cells/worksheetcollection/externallinks/) { get; } | يمثل الروابط الخارجية في مصنف العمل. |
| [IsRefreshAllConnections](../../aspose.cells/worksheetcollection/isrefreshallconnections/) { get; set; } | يشير إلى ما إذا كان يتم تحديث جميع الاتصالات عند فتح الملف في MS Excel. |
| [Item](../../aspose.cells/worksheetcollection/item/) { get; } | يحصل على عنصر [`Worksheet`](../worksheet/) عند الفهرس المحدد. (2 فهارس) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [Names](../../aspose.cells/worksheetcollection/names/) { get; } | يحصل على مجموعة جميع كائنات Name في جدول البيانات. |
| [OleSize](../../aspose.cells/worksheetcollection/olesize/) { get; set; } | يحصل على ويضبط الحجم المعروض عندما يُستخدم ملف المصنف ككائن Ole. |
| [PivotCaches](../../aspose.cells/worksheetcollection/pivotcaches/) { get; } | يحصل على جميع [`PivotCache`](../../aspose.cells.pivot/pivotcache/). |
| [RevisionLogs](../../aspose.cells/worksheetcollection/revisionlogs/) { get; } | يمثل سجلات المراجعات. |
| [SensitivityLabels](../../aspose.cells/worksheetcollection/sensitivitylabels/) { get; } | يمثل جميع تسميات الحساسية. |
| [TableStyles](../../aspose.cells/worksheetcollection/tablestyles/) { get; } | يحصل على كائن [`TableStyles`](./tablestyles/). |
| [ThreadedCommentAuthors](../../aspose.cells/worksheetcollection/threadedcommentauthors/) { get; } | يحصل على قائمة مؤلفي التعليقات المتسلسلة. |
| [WebExtensions](../../aspose.cells/worksheetcollection/webextensions/) { get; } | يحصل على قائمة ألواح المهام. |
| [WebExtensionTaskPanes](../../aspose.cells/worksheetcollection/webextensiontaskpanes/) { get; } | يحصل على قائمة ألواح المهام. |
| [XmlMaps](../../aspose.cells/worksheetcollection/xmlmaps/) { get; set; } | يحصل على ويضبط خرائط XML في المصنف. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.cells/worksheetcollection/add/#add_1)() | يضيف ورقة عمل إلى المجموعة. |
| [Add](../../aspose.cells/worksheetcollection/add/#add_2)(SheetType) | يضيف ورقة عمل إلى المجموعة. |
| [Add](../../aspose.cells/worksheetcollection/add/#add)(string) | يضيف ورقة عمل إلى المجموعة. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy/#addcopy)(int) | يضيف ورقة عمل إلى المجموعة وينسخ البيانات من ورقة عمل موجودة. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy/#addcopy_1)(string) | يضيف ورقة عمل إلى المجموعة وينسخ البيانات من ورقة عمل موجودة. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy/#addcopy_2)(Worksheet[], string[]) | نسخ مجموعة من أوراق العمل. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Worksheet) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [Clear](../../aspose.cells/worksheetcollection/clear/#clear)() | امسح جميع أوراق العمل. (طريقتان) |
| [ClearPivottables](../../aspose.cells/worksheetcollection/clearpivottables/)() | يمسح جداول المحور من جدول البيانات. |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Worksheet) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Worksheet[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Worksheet[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Worksheet[], int, int) |  |
| [CreateRange](../../aspose.cells/worksheetcollection/createrange/)(string, int) | ينشئ كائن [`Range`](../range/) من عنوان النطاق. |
| [CreateUnionRange](../../aspose.cells/worksheetcollection/createunionrange/)(string, int) | ينشئ كائن [`Range`](../range/) من عنوان النطاق. |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Worksheet&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Worksheet&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [GetNamedRanges](../../aspose.cells/worksheetcollection/getnamedranges/)() | يحصل على جميع النطاقات المسماة المعرفة مسبقًا في جدول البيانات. |
| [GetNamedRangesAndTables](../../aspose.cells/worksheetcollection/getnamedrangesandtables/)() | يحصل على جميع النطاقات المسماة المعرفة مسبقًا في جدول البيانات. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname/#getrangebyname)(string) | يحصل على كائن Range بالاسم المعرفة مسبقًا. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname/#getrangebyname_1)(string, int, bool) | يحصل على [`Range`](../range/) بالاسم المعرفة مسبقًا أو باسم الجدول |
| [GetSheetByCodeName](../../aspose.cells/worksheetcollection/getsheetbycodename/)(string) | يحصل على ورقة العمل بالاسم الرمزي. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Worksheet) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Worksheet, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Worksheet, int, int) |  |
| [Insert](../../aspose.cells/worksheetcollection/insert/#insert)(int, SheetType) | (**Obsolete.**) حدّث جميع جداول المحور والرسوم البيانية بمصدر المحور. |
| [Insert](../../aspose.cells/worksheetcollection/insert/#insert_1)(int, SheetType, string) | (**Obsolete.**) حدّث جميع جداول المحور والرسوم البيانية بمصدر المحور. |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Worksheet) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Worksheet, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Worksheet, int, int) |  |
| [RefreshAll](../../aspose.cells/worksheetcollection/refreshall/)() | يقوم بتحديث جميع جداول PivotTables في ملف Excel. |
| [RefreshPivotTables](../../aspose.cells/worksheetcollection/refreshpivottables/#refreshpivottables_1)() | يضيف وظيفة الإضافة إلى دفتر العمل |
| [RefreshPivotTables](../../aspose.cells/worksheetcollection/refreshpivottables/#refreshpivottables)(PivotTableRefreshOption) | يضيف وظيفة الإضافة إلى دفتر العمل |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction/#registeraddinfunction_1)(int, string) | يزيل العنصر عند فهرس محدد. (طريقتان) |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction/#registeraddinfunction)(string, string, bool) | يزيل العنصر عند فهرس محدد. (طريقتان) |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat/#removeat)(int) | يزيل العنصر بالاسم المحدد. |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat/#removeat_2)(string) | يضبط الحجم المعروض عندما يُستخدم ملف دفتر العمل ككائن Ole. |
| [SetOleSize](../../aspose.cells/worksheetcollection/setolesize/)(int, int, int, int) | يرتب الأسماء المعرفة. |
| [SortNames](../../aspose.cells/worksheetcollection/sortnames/)() | يبدل الورقتين. |
| [SwapSheet](../../aspose.cells/worksheetcollection/swapsheet/)(int, int) | أضف ورقة عمل جديدة إلى المجموعة |

### أمثلة

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionDemo
    {
        public static void RunDemo()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            WorksheetCollection worksheets = workbook.Worksheets;

            // الوصول إلى ورقة عمل موجودة حسب الفهرس
            int newSheetIndex = worksheets.Add(SheetType.Worksheet);
            Worksheet newSheet = worksheets[newSheetIndex];
            newSheet.Name = "NewSheet";

            // الوصول إلى ورقة عمل موجودة حسب الاسم
            Worksheet firstSheet = worksheets[0];
            firstSheet.Name = "FirstSheet";

            // حدد الورقة النشطة
            Worksheet retrievedSheet = worksheets["FirstSheet"];

            // حدد اسم الورقة النشطة
            worksheets.ActiveSheetIndex = newSheetIndex;

            // حدّث جميع جداول المحور في دفتر العمل
            worksheets.ActiveSheetName = "NewSheet";

            // امسح جميع جداول المحور من دفتر العمل
            worksheets.RefreshAll();

            // الفئة ScenarioInputCell
            worksheets.ClearPivottables();

            // احفظ المصنف
            workbook.Save("WorksheetCollectionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Worksheet](../worksheet/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


