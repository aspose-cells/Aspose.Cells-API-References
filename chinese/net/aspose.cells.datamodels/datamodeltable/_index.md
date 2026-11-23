---
title: "类 DataModelTable"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.DataModels.DataModelTable 类。表示电子表格数据模型中单个表的属性"
type: docs
url: /zh/net/aspose.cells.datamodels/datamodeltable/
---
## DataModelTable class

表示电子表格数据模型中单个表的属性。

```csharp
public class DataModelTable
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [ConnectionName](../../aspose.cells.datamodels/datamodeltable/connectionname/) { get; } | 获取数据模型表的连接名称。 |
| [Id](../../aspose.cells.datamodels/datamodeltable/id/) { get; } | 获取数据模型表的 ID。 |
| [Name](../../aspose.cells.datamodels/datamodeltable/name/) { get; } | 获取数据模型表的名称。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using Aspose.Cells.Tables;
    using Aspose.Cells.Pivot;
    using System;

    public class DataModelsClassDataModelTableDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加示例数据以创建表
            worksheet.Cells["A1"].PutValue("ProductID");
            worksheet.Cells["B1"].PutValue("ProductName");
            worksheet.Cells["A2"].PutValue(101);
            worksheet.Cells["B2"].PutValue("Laptop");
            worksheet.Cells["A3"].PutValue(102);
            worksheet.Cells["B3"].PutValue("Monitor");

            // 创建 ListObject（表）
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "ProductsTable";

            // 访问 DataModelTable
            DataModelTable dataModelTable = workbook.DataModel.Tables[0];

            // 显示 DataModelTable 属性
            Console.WriteLine("Data Model Table Properties:");
            Console.WriteLine($"ID: {dataModelTable.Id}");
            Console.WriteLine($"Name: {dataModelTable.Name}");
            Console.WriteLine($"Connection Name: {dataModelTable.ConnectionName}");

            // 使用 DataModelTable 创建数据透视表
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable1", "A1", dataModelTable.Name);
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "ProductName");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "ProductID");

            // 保存工作簿
            workbook.Save("DataModelTableDemo.xlsx");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)


