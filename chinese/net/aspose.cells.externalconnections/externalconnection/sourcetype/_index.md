---
title: "ExternalConnection.SourceType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ExternalConnection property. 获取或设置外部连接的数据源类型"
type: docs
url: /zh/net/aspose.cells.externalconnections/externalconnection/sourcetype/
---
## ExternalConnection.SourceType property

获取或设置外部连接的数据源类型。

```csharp
public ConnectionDataSourceType SourceType { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertySourceTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 添加工作表并创建数据透视表
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["B3"].PutValue(2000);
            
            // 创建数据透视表
            int index = sheet.PivotTables.Add("A1:B3", "C3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = sheet.PivotTables[index];
            
            // 获取外部连接
            ExternalConnection conn = pivotTable.GetSourceDataConnections()[0];
            
            // 演示 SourceType 属性
            Console.WriteLine("Connection Source Type: " + conn.SourceType);
            
            // 修改连接属性
            conn.Name = "TestConnection";
            conn.SourceType = ConnectionDataSourceType.OLEDBDataModel;
            
            // 输出已修改的属性
            Console.WriteLine("Modified Connection Name: " + conn.Name);
            Console.WriteLine("Modified Source Type: " + conn.SourceType);
        }
    }
}
```

### 另请参见

* enum [ConnectionDataSourceType](../../connectiondatasourcetype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


