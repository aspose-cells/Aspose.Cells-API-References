---
title: "使用 DataModelTable 的连接创建数据透视表"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "注意：ConnectionName 是只读的，无法设置"
type: docs
url: /zh/net/aspose.cells.datamodels/datamodeltable/connectionname/
---
## DataModelTable.ConnectionName property

获取数据模型表的连接名称。

```csharp
public string ConnectionName { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using Aspose.Cells.Tables;
    using Aspose.Cells.Pivot;
    using System;

    public class DataModelTablePropertyConnectionNameDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加示例数据以创建表
            worksheet.Cells["A1"].PutValue("OrderID");
            worksheet.Cells["B1"].PutValue("Customer");
            worksheet.Cells["A2"].PutValue(1001);
            worksheet.Cells["B2"].PutValue("John Doe");
            worksheet.Cells["A3"].PutValue(1002);
            worksheet.Cells["B3"].PutValue("Jane Smith");

            // 创建 ListObject（表）
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "OrdersTable";

            // 访问 DataModelTable
            DataModelTable dataModelTable = workbook.DataModel.Tables[0];

            // 显示当前的 ConnectionName 值
            Console.WriteLine("Current ConnectionName: " + dataModelTable.ConnectionName);

            // 使用 DataModelTable 的连接创建数据透视表
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotReport");
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable1", "A1", dataModelTable.Name);
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Customer");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "OrderID");

            // 注意：ConnectionName 是只读的，因此我们无法设置它
            // 这演示了如何使用现有的连接名称
            if (!string.IsNullOrEmpty(dataModelTable.ConnectionName))
            {
                Console.WriteLine("This table is connected via: " + dataModelTable.ConnectionName);
            }

            // 保存工作簿
            workbook.Save("DataModelTableConnectionNameDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [DataModelTable](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


