---
title: "ExternalConnection.CommandType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ExternalConnection 属性。指定 OLE DB 命令类型。1. 查询指定立方体名称 2. 查询指定 SQL 语句 3. 查询指定表名 4. 查询指定已提供默认信息，由提供程序自行解释。5. 查询针对基于 Web 的 List Data Provider"
type: docs
url: /zh/net/aspose.cells.externalconnections/externalconnection/commandtype/
---
## ExternalConnection.CommandType property

指定 OLE DB 命令类型。1. 查询指定立方体名称 2. 查询指定 SQL 语句 3. 查询指定表名 4. 查询指定已提供默认信息，由提供程序自行解释。5. 查询针对基于 Web 的 List Data Provider。

```csharp
public virtual OLEDBCommandType CommandType { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyCommandTypeDemo
    {
        public static void Run()
        {
            // 使用示例数据创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 添加示例数据
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1500);

            // 创建数据透视表
            int index = worksheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[index];

            // 获取外部连接
            ExternalConnection conn = pivotTable.GetSourceDataConnections()[0];
            
            // 演示 CommandType 属性
            Console.WriteLine("Original CommandType: " + conn.CommandType);
            
            // 更改并显示 CommandType
            conn.CommandType = Aspose.Cells.ExternalConnections.OLEDBCommandType.TableName;
            Console.WriteLine("Modified CommandType: " + conn.CommandType);
            
            // 保存工作簿
            workbook.Save("ExternalConnectionCommandTypeDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [OLEDBCommandType](../../oledbcommandtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


