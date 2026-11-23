---
title: "PivotTable.GetSourceDataConnections"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotTable 方法。获取外部连接数据源"
type: docs
url: /zh/net/aspose.cells.pivot/pivottable/getsourcedataconnections/
---
## PivotTable.GetSourceDataConnections method

获取外部连接数据源。

```csharp
public ExternalConnection[] GetSourceDataConnections()
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetSourceDataConnectionsDemo
    {
        public static void Run()
        {
            // 使用示例数据创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 添加示例数据
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            
            // 创建数据透视表
            int index = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // 获取源数据连接
            ExternalConnection[] connections = pivotTable.GetSourceDataConnections();
            
            // 显示连接信息
            if (connections.Length > 0)
            {
                ExternalConnection conn = connections[0];
                Console.WriteLine("Connection Name: " + conn.Name);
                Console.WriteLine("Class Type: " + conn.ClassType);
                Console.WriteLine("Source Type: " + conn.SourceType);
                Console.WriteLine("Command: " + conn.Command);
            }
            
            // 保存工作簿
            workbook.Save("PivotTableSourceConnections.xlsx");
        }
    }
}
```

### 另请参见

* class [ExternalConnection](../../../aspose.cells.externalconnections/externalconnection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


