---
title: "الفئة PowerQueryFormulaItemCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.QueryTables.PowerQueryFormulaItemCollection. تمثل جميع عناصر صيغة استعلام الطاقة"
type: docs
url: /ar/net/aspose.cells.querytables/powerqueryformulaitemcollection/
---
## PowerQueryFormulaItemCollection class

يمثل جميع عناصر صيغة Power Query.

```csharp
public class PowerQueryFormulaItemCollection : CollectionBase<PowerQueryFormulaItem>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.querytables/powerqueryformulaitemcollection/item/) { get; } | يحصل على [`PowerQueryFormulaItem`](../powerqueryformulaitem/) حسب الفهرس في القائمة. (مؤشرين) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PowerQueryFormulaItem) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PowerQueryFormulaItem, IComparer&lt;PowerQueryFormulaItem&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, PowerQueryFormulaItem, IComparer&lt;PowerQueryFormulaItem&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(PowerQueryFormulaItem) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PowerQueryFormulaItem[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PowerQueryFormulaItem[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, PowerQueryFormulaItem[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PowerQueryFormulaItem) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PowerQueryFormulaItem, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PowerQueryFormulaItem, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PowerQueryFormulaItem) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PowerQueryFormulaItem, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PowerQueryFormulaItem, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class QueryTablesClassPowerQueryFormulaItemCollectionDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات عينة Power Query (محاكاة لأننا لا نستطيع إنشاء صيغ PQ فعلية برمجياً)
            // عادةً ستقوم بتحميل ملف موجود يحتوي على صيغ PQ
            string sourcePath = "example.xlsm";
            try
            {
                workbook = new Workbook(sourcePath);
            }
            catch
            {
                Console.WriteLine("File not found. Using new workbook for demonstration.");
                return;
            }

            // الوصول إلى صيغ Power Query
            PowerQueryFormulaCollection pqFormulas = workbook.DataMashup.PowerQueryFormulas;
            
            if (pqFormulas.Count > 0)
            {
                // احصل على أول صيغة Power Query
                PowerQueryFormula formula = pqFormulas[0];
                Console.WriteLine("Formula Name: {0}", formula.Name);

                // الوصول إلى عناصر الصيغة
                PowerQueryFormulaItemCollection items = formula.PowerQueryFormulaItems;
                Console.WriteLine("Number of items: {0}", items.Count);

                if (items.Count > 0)
                {
                    // عرض العنصر الأول
                    PowerQueryFormulaItem item = items[0];
                    Console.WriteLine("Item Name: {0}", item.Name);
                    Console.WriteLine("Item Value: {0}", item.Value);
                }
            }
            else
            {
                Console.WriteLine("No Power Query formulas found in the workbook.");
            }
        }
    }
}
```

### انظر أيضًا

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [PowerQueryFormulaItem](../powerqueryformulaitem/)
* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


