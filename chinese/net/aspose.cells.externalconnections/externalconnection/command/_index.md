---
title: "ExternalConnection.Command"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ExternalConnection 属性。包含要传递给数据提供程序 API 的数据库命令字符串，该 API 将与外部源交互以检索数据"
type: docs
url: /zh/net/aspose.cells.externalconnections/externalconnection/command/
---
## ExternalConnection.Command property

包含要传递给数据提供程序 API 的数据库命令的字符串，该 API 将与外部源交互以检索数据

```csharp
public virtual string Command { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyCommandDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 添加工作表和一些示例数据
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(150);
            
            // 创建表范围
            var range = worksheet.Cells.CreateRange("A1:B3");
            
            // 使用该范围作为源创建数据透视表
            int index = worksheet.PivotTables.Add("D1", "A1:B3", "PivotTable1");
            var pivotTable = worksheet.PivotTables[index];
            
            // 获取外部连接
            ExternalConnection[] connections = pivotTable.GetSourceDataConnections();
            
            // 显示连接的 Command 属性
            if (connections.Length > 0)
            {
                Console.WriteLine("Connection Command: " + connections[0].Command);
            }
            
            // 保存工作簿
            workbook.Save("ExternalConnectionCommandDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


