---
title: "DataModelTable.Id"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "DataModelTable 属性。获取数据模型表的 id"
type: docs
url: /zh/net/aspose.cells.datamodels/datamodelrelationship/primarykeycolumn/
---
## DataModelRelationship.PrimaryKeyColumn property

获取此关系的主键表列的名称。

```csharp
public string PrimaryKeyColumn { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelRelationshipPropertyPrimaryKeyColumnDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加示例数据以创建有意义的上下文
            worksheet.Cells["A1"].PutValue("Orders");
            worksheet.Cells["A2"].PutValue("OrderID");
            worksheet.Cells["A3"].PutValue("CustomerID");

            worksheet.Cells["C1"].PutValue("Customers");
            worksheet.Cells["C2"].PutValue("CustomerID");
            worksheet.Cells["C3"].PutValue("CustomerName");

            try
            {
                // 如果存在，访问第一个关系
                DataModelRelationship relationship = workbook.DataModel?.Relationships?[0];

                if (relationship != null)
                {
                    // 获取 DataModelTable（在工作簿中为只读）
                    Console.WriteLine("Primary Key Column: " + relationship.PrimaryKeyColumn);
                }
                else
                {
                    Console.WriteLine("No relationships found in the data model.");
                }

                // 保存工作簿
                workbook.Save("PrimaryKeyColumnDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [DataModelRelationship](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


