---
title: "DataModelTableCollection.Item"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "DataModelTableCollection 属性。获取集合中位置对应的数据模型表"
type: docs
url: /zh/net/aspose.cells.datamodels/datamodeltablecollection/item/
---
## DataModelTableCollection indexer (1 of 2)

获取集合中位置对应的数据模型表。

```csharp
public DataModelTable this[int index] { get; }
```

| 参数 | 描述 |
| --- | --- |
| 索引 | 集合中的位置。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using Aspose.Cells.Tables;
    using System;

    public class DataModelTableCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为表创建示例数据
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Jane");

            // 创建表
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "EmployeeTable";

            // 访问 DataModelTableCollection
            DataModelTableCollection dataModelTables = workbook.DataModel.Tables;

            // 演示读取 Item 属性（索引器）
            Console.WriteLine("Number of tables: " + dataModelTables.Count);
            for (int i = 0; i < dataModelTables.Count; i++)
            {
                DataModelTable tableItem = dataModelTables[i]; // Using Item property
                Console.WriteLine($"Table {i}: {tableItem.Name}");
            }

            // 添加另一张表以演示多个项目
            worksheet.Cells["D1"].PutValue("DeptID");
            worksheet.Cells["E1"].PutValue("Department");
            worksheet.Cells["D2"].PutValue(101);
            worksheet.Cells["E2"].PutValue("HR");
            int secondTableIndex = worksheet.ListObjects.Add(3, 0, 1, 1, true);
            worksheet.ListObjects[secondTableIndex].DisplayName = "DepartmentTable";

            // 显示更新后的集合
            Console.WriteLine("\nAfter adding second table:");
            for (int i = 0; i < dataModelTables.Count; i++)
            {
                Console.WriteLine($"Table {i}: {dataModelTables[i].Name}");
            }

            // 保存工作簿
            workbook.Save("DataModelTableCollectionItemIndexDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [DataModelTable](../../datamodeltable/)
* class [DataModelTableCollection](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)

---

## DataModelTableCollection indexer (2 of 2)

通过名称获取数据模型表。

```csharp
public DataModelTable this[string name] { get; }
```

| 参数 | 描述 |
| --- | --- |
| 名称 | 数据模型表的名称。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using Aspose.Cells.Tables;
    using System;

    public class DataModelTableCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Widget");
            worksheet.Cells["B2"].PutValue(49.99);

            int tableIndex = worksheet.ListObjects.Add(0, 0, 1, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "InventoryTable";

            DataModelTableCollection dataModelTables = workbook.DataModel.Tables;
            DataModelTable dataModelTable = dataModelTables["InventoryTable"];

            Console.WriteLine("Initial Table Name: " + dataModelTable.Name);

            worksheet.ListObjects[0].DisplayName = "UpdatedInventory";
            dataModelTable = dataModelTables["UpdatedInventory"];
            Console.WriteLine("Updated Table Name: " + dataModelTable.Name);

            workbook.Save("DataModelTableCollectionItemDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [DataModelTable](../../datamodeltable/)
* class [DataModelTableCollection](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


