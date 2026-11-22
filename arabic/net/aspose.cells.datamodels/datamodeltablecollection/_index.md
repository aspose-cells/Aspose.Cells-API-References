---
title: "الفئة DataModelTableCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.DataModels.DataModelTableCollection. تمثل قائمة جدول نموذج البيانات"
type: docs
url: /ar/net/aspose.cells.datamodels/datamodeltablecollection/
---
## DataModelTableCollection class

يمثل قائمة جدول نموذج البيانات.

```csharp
public class DataModelTableCollection : CollectionBase<DataModelTable>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.datamodels/datamodeltablecollection/item/) { get; } | يحصل على جدول نموذج البيانات حسب موضع المجموعة. (مؤشرين) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DataModelTable) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DataModelTable, IComparer&lt;DataModelTable&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, DataModelTable, IComparer&lt;DataModelTable&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(DataModelTable) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(DataModelTable[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(DataModelTable[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, DataModelTable[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;DataModelTable&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;DataModelTable&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;DataModelTable&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;DataModelTable&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;DataModelTable&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;DataModelTable&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;DataModelTable&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;DataModelTable&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;DataModelTable&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;DataModelTable&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DataModelTable) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DataModelTable, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DataModelTable, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DataModelTable) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DataModelTable, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DataModelTable, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using Aspose.Cells.Tables;
    using System;

    public class DataModelsClassDataModelTableCollectionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء بيانات عينة للجدول الأول
            worksheet.Cells["A1"].PutValue("OrderID");
            worksheet.Cells["B1"].PutValue("Customer");
            worksheet.Cells["A2"].PutValue(1001);
            worksheet.Cells["B2"].PutValue("Company A");
            worksheet.Cells["A3"].PutValue(1002);
            worksheet.Cells["B3"].PutValue("Company B");

            // إنشاء الجدول الأول
            int firstTableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject firstTable = worksheet.ListObjects[firstTableIndex];
            firstTable.DisplayName = "OrdersTable";

            // إنشاء بيانات عينة للجدول الثاني
            worksheet.Cells["D1"].PutValue("ProductID");
            worksheet.Cells["E1"].PutValue("ProductName");
            worksheet.Cells["D2"].PutValue(101);
            worksheet.Cells["E2"].PutValue("Laptop");
            worksheet.Cells["D3"].PutValue(102);
            worksheet.Cells["E3"].PutValue("Monitor");

            // إنشاء الجدول الثاني
            int secondTableIndex = worksheet.ListObjects.Add(3, 0, 2, 1, true);
            ListObject secondTable = worksheet.ListObjects[secondTableIndex];
            secondTable.DisplayName = "ProductsTable";

            // الوصول إلى DataModelTableCollection
            DataModelTableCollection dataModelTables = workbook.DataModel.Tables;

            // إظهار الوصول إلى الجداول حسب الفهرس
            Console.WriteLine("Tables accessed by index:");
            for (int i = 0; i < dataModelTables.Count; i++)
            {
                Console.WriteLine($"Table {i}: {dataModelTables[i].Name}");
            }

            // إظهار الوصول إلى الجداول حسب الاسم
            Console.WriteLine("\nTables accessed by name:");
            DataModelTable ordersTable = dataModelTables["OrdersTable"];
            DataModelTable productsTable = dataModelTables["ProductsTable"];
            Console.WriteLine($"Orders table exists: {ordersTable != null}");
            Console.WriteLine($"Products table exists: {productsTable != null}");

            // احفظ المصنف
            workbook.Save("DataModelTableCollectionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [DataModelTable](../datamodeltable/)
* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)


