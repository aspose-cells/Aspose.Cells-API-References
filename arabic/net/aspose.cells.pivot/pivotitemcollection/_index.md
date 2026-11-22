---
title: "الفئة PivotItemCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Pivot.PivotItemCollection. تمثل جميع كائنات PivotItem في PivotField"
type: docs
url: /ar/net/aspose.cells.pivot/pivotitemcollection/
---
## PivotItemCollection class

تمثل جميع كائنات [`PivotItem`](../pivotitem/) في PivotField.

```csharp
public class PivotItemCollection : CollectionBase<PivotItem>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.pivot/pivotitemcollection/item/) { get; } | يحصل على كائن PivotItem في الفهرس المحدد. (2 indexers) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotItem) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotItem, IComparer&lt;PivotItem&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, PivotItem, IComparer&lt;PivotItem&gt;) |  |
| [ChangeitemsOrder](../../aspose.cells.pivot/pivotitemcollection/changeitemsorder/)(int, int) | (**Obsolete.**) يغيّر مباشرةً ترتيب العنصرين. |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(PivotItem) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotItem[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotItem[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, PivotItem[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;PivotItem&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;PivotItem&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;PivotItem&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;PivotItem&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;PivotItem&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;PivotItem&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;PivotItem&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;PivotItem&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;PivotItem&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;PivotItem&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [HideAllDetail](../../aspose.cells.pivot/pivotitemcollection/hidealldetail/)(bool) | (**Obsolete.**) يحدد ما إذا كان يجب إخفاء جميع تفاصيل جميع PivotItems في حقل محوري. أي طي/توسيع هذا الحقل. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotItem) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotItem, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotItem, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotItem) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotItem, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotItem, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
| [SwapItem](../../aspose.cells.pivot/pivotitemcollection/swapitem/)(int, int) | تبديل العنصرين مباشرةً. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemCollectionDemo
    {
        public static void PivotItemCollectionExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات إلى ورقة العمل
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[3, 0].Value = "Cherry";
            worksheet.Cells[4, 0].Value = "Date";

            worksheet.Cells[0, 1].Value = "Quantity";
            worksheet.Cells[1, 1].Value = 10;
            worksheet.Cells[2, 1].Value = 20;
            worksheet.Cells[3, 1].Value = 30;
            worksheet.Cells[4, 1].Value = 40;

            // أضف جدولًا محوريًا إلى ورقة العمل
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // إضافة حقول إلى الجدول المحوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Quantity

            // الوصول إلى PivotField و PivotItems الخاصة به
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            // عرض عدد عناصر pivot
            Console.WriteLine("Pivot Items Count: " + pivotItems.Count);

            // التنقل عبر عناصر pivot وعرض أسمائها
            foreach (PivotItem item in pivotItems)
            {
                Console.WriteLine("Pivot Item: " + item.Name);
            }

            // تغيير ترتيب عناصر pivot
            pivotItems.ChangeitemsOrder(0, 2);

            // احفظ المصنف
            workbook.Save("PivotItemCollectionExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [PivotItem](../pivotitem/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


