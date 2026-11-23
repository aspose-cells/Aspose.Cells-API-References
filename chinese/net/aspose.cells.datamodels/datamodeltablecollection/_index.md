---
title: "类 DataModelTableCollection"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.DataModels.DataModelTableCollection 类。表示数据模型表的列表"
type: docs
url: /zh/net/aspose.cells.datamodels/datamodeltablecollection/
---
## DataModelTableCollection class

表示数据模型表的列表。

```csharp
public class DataModelTableCollection : CollectionBase<DataModelTable>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.datamodels/datamodeltablecollection/item/) { get; } | 通过集合的位置获取数据模型表。（2 个索引器） |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## 方法

| 名称 | 描述 |
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

### 示例

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
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为第一个表创建示例数据
            worksheet.Cells["A1"].PutValue("OrderID");
            worksheet.Cells["B1"].PutValue("Customer");
            worksheet.Cells["A2"].PutValue(1001);
            worksheet.Cells["B2"].PutValue("Company A");
            worksheet.Cells["A3"].PutValue(1002);
            worksheet.Cells["B3"].PutValue("Company B");

            // 创建第一个表
            int firstTableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject firstTable = worksheet.ListObjects[firstTableIndex];
            firstTable.DisplayName = "OrdersTable";

            // 为第二个表创建示例数据
            worksheet.Cells["D1"].PutValue("ProductID");
            worksheet.Cells["E1"].PutValue("ProductName");
            worksheet.Cells["D2"].PutValue(101);
            worksheet.Cells["E2"].PutValue("Laptop");
            worksheet.Cells["D3"].PutValue(102);
            worksheet.Cells["E3"].PutValue("Monitor");

            // 创建第二个表
            int secondTableIndex = worksheet.ListObjects.Add(3, 0, 2, 1, true);
            ListObject secondTable = worksheet.ListObjects[secondTableIndex];
            secondTable.DisplayName = "ProductsTable";

            // 访问 DataModelTableCollection
            DataModelTableCollection dataModelTables = workbook.DataModel.Tables;

            // 演示按索引访问表
            Console.WriteLine("Tables accessed by index:");
            for (int i = 0; i < dataModelTables.Count; i++)
            {
                Console.WriteLine($"Table {i}: {dataModelTables[i].Name}");
            }

            // 演示按名称访问表
            Console.WriteLine("\nTables accessed by name:");
            DataModelTable ordersTable = dataModelTables["OrdersTable"];
            DataModelTable productsTable = dataModelTables["ProductsTable"];
            Console.WriteLine($"Orders table exists: {ordersTable != null}");
            Console.WriteLine($"Products table exists: {productsTable != null}");

            // 保存工作簿
            workbook.Save("DataModelTableCollectionDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [DataModelTable](../datamodeltable/)
* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)


