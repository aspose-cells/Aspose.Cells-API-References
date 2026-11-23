---
title: "ExternalConnection.ConnectionString"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ExternalConnection property. 连接信息字符串用于与 OLE DB 或 ODBC 数据源建立联系"
type: docs
url: /zh/net/aspose.cells.externalconnections/externalconnection/connectionstring/
---
## ExternalConnection.ConnectionString property

连接信息字符串用于与 OLE DB 或 ODBC 数据源建立联系。

```csharp
public virtual string ConnectionString { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyConnectionStringDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 添加工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 创建示例数据
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1500);
            
            // 创建数据透视表
            int index = worksheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // 获取数据连接
            ExternalConnection[] connections = pivotTable.GetSourceDataConnections();
            
            // 如果存在则显示连接字符串
            if (connections.Length > 0)
            {
                Console.WriteLine("Connection String: " + connections[0].ConnectionString);
            }
            
            // 保存工作簿
            workbook.Save("PivotTableWithConnection.xlsx");
        }
    }
}
```

### 另请参见

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


