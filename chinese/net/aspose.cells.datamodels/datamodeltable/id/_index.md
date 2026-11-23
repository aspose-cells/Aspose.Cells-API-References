---
title: "显示当前 Id 值"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "注意：Id 属性是只读的，无法设置"
type: docs
url: /zh/net/aspose.cells.datamodels/datamodeltable/id/
---
## DataModelTable.Id property

获取数据模型表的 ID。

```csharp
public string Id { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using Aspose.Cells.Tables;
    using System;

    public class DataModelTablePropertyIdDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加示例数据以创建表
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Item 2");

            // 创建 ListObject（表）
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];

            // 这演示了如何访问和使用现有的 Id
            DataModelTable dataModelTable = workbook.DataModel.Tables[0];

            // 示例用法：在处理多个表时比较表 ID
            Console.WriteLine("Current DataModelTable Id: " + dataModelTable.Id);

            // DataModelTable.Name
            // DataModelTable 属性。获取数据模型表的名称

            // DataModelTable.ConnectionName
            DataModelTable secondTable = null;
            if (workbook.DataModel.Tables.Count > 1)
            {
                secondTable = workbook.DataModel.Tables[1];
                if (dataModelTable.Id != secondTable.Id)
                {
                    Console.WriteLine("Different table IDs detected");
                }
            }

            // 保存工作簿
            workbook.Save("DataModelTableIdDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [DataModelTable](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


