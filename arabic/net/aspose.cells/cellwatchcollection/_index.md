---
title: "Class CellWatchCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.CellWatchCollection class. يمثل مجموعة الخلايا في هذه ورقة العمل التي يتم مراقبتها في نافذة المراقبة"
type: docs
url: /ar/net/aspose.cells/cellwatchcollection/
---
## CellWatchCollection class

يمثل مجموعة الخلايا في ورقة العمل هذه التي يتم مراقبتها في 'نافذة المراقبة'.

```csharp
public class CellWatchCollection : CollectionBase<CellWatch>
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [CellWatchCollection](cellwatchcollection/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/cellwatchcollection/item/) { get; } | يحصل ويضبط [`CellWatch`](../cellwatch/) حسب الفهرس. (مؤشرين) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.cells/cellwatchcollection/add/#add_1)(string) | يضيف [`CellWatch`](../cellwatch/) باسم الخلية. |
| [Add](../../aspose.cells/cellwatchcollection/add/#add)(int, int) | يضيف [`CellWatch`](../cellwatch/) مع صف وعمود. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CellWatch) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CellWatch, IComparer&lt;CellWatch&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, CellWatch, IComparer&lt;CellWatch&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(CellWatch) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CellWatch[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CellWatch[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, CellWatch[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;CellWatch&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;CellWatch&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;CellWatch&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;CellWatch&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;CellWatch&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;CellWatch&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;CellWatch&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;CellWatch&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;CellWatch&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;CellWatch&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CellWatch) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CellWatch, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CellWatch, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CellWatch) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CellWatch, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CellWatch, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellWatchCollectionDemo
    {
        public static void CellWatchCollectionExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();
            
            // احصل على الـWorksheet الأول
            Worksheet sheet = workbook.Worksheets[0];
            
            // أضف عنصر مراقبة الخلية إلى نافذة المراقبة
            int watchIndex = sheet.CellWatches.Add("B2");
            
            // الوصول إلى CellWatchCollection
            CellWatchCollection cellWatches = sheet.CellWatches;
            
            // الوصول إلى عنصر CellWatch المضاف
            CellWatch cellWatch = cellWatches[watchIndex];
            
            // عرض خصائص عنصر CellWatch
            Console.WriteLine("Cell Watch Details:");
            Console.WriteLine($"Row: {cellWatch.Row}");
            Console.WriteLine($"Column: {cellWatch.Column}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            
            // تعديل خصائص عنصر CellWatch
            cellWatch.Row = 1;
            cellWatch.Column = 1;
            cellWatch.CellName = "A2";
            
            // عرض الخصائص المعدلة لعنصر CellWatch
            Console.WriteLine("Modified Cell Watch Details:");
            Console.WriteLine($"Row: {cellWatch.Row}");
            Console.WriteLine($"Column: {cellWatch.Column}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            
            // احفظ المصنف
            workbook.Save("CellWatchCollectionExample.xlsx");
            workbook.Save("CellWatchCollectionExample.pdf");
        }
    }
}
```

### انظر أيضًا

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [CellWatch](../cellwatch/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


