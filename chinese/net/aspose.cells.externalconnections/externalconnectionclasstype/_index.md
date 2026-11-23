---
title: "枚举 ExternalConnectionClassType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.ExternalConnections.ExternalConnectionClassType 枚举。表示连接的类型"
type: docs
url: /zh/net/aspose.cells.externalconnections/externalconnectionclasstype/
---
## ExternalConnectionClassType enumeration

表示连接的类型

```csharp
public enum ExternalConnectionClassType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Database | `0` | ODBC 或 OLE DB |
| WebQuery | `1` | Web 查询 |
| TextBased | `2` | 基于文本 |
| DataModel | `3` | 数据模型 |
| Unkown | `4` |  |

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class ExternalConnectionsClassExternalConnectionClassTypeDemo
    {
        public static void Run()
        {
            // 使用示例数据创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 为连接添加示例数据
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue(i - 1);
                worksheet.Cells[$"B{i}"].PutValue($"Name_{i - 1}");
            }

            // 使用这些数据创建数据透视表
            int pivotIndex = worksheet.PivotTables.Add("A1:B10", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // 获取外部连接并演示其属性
            ExternalConnection conn = workbook.DataConnections[0];
            
            Console.WriteLine($"Connection Name: {conn.Name}");
            Console.WriteLine($"Class Type: {conn.ClassType}");
            Console.WriteLine($"Source Type: {conn.SourceType}");
            Console.WriteLine($"Command: {conn.Command}");
            Console.WriteLine($"Connection File: {conn.ConnectionFile ?? "null"}");
            Console.WriteLine($"Connection String: {conn.ConnectionString ?? "null"}");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


