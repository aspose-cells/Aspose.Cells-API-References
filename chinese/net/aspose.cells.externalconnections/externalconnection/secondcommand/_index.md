---
title: "ExternalConnection.SecondCommand"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ExternalConnection property. 指定一个在使用 PivotTable 服务器分页字段时会被保留的第二个命令文本字符串。对于 ODBC 连接，serverCommand 通常比 command 更宽泛，前者不包含 WHERE 子句。基于这两个命令 Command 和 ServerCommand，可以填充参数 UI 并构建参数化查询。"
type: docs
url: /zh/net/aspose.cells.externalconnections/externalconnection/secondcommand/
---
## ExternalConnection.SecondCommand property

指定在使用 PivotTable 服务器页面字段时持久化的第二个命令文本字符串。对于 ODBC 连接，serverCommand 通常比 command 更宽泛（前者不包含 WHERE 子句）。基于这两个命令（Command 和 ServerCommand），可以填充参数 UI 并构建参数化查询。

```csharp
public virtual string SecondCommand { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySecondCommandDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            try
            {
                // 访问第一个外部连接（假设存在）
                ExternalConnection connection = workbook.DataConnections[0];
                
                // 显示当前 SecondCommand 值（读取操作）
                Console.WriteLine("Initial SecondCommand value: " + connection.SecondCommand);
                
                // 设置新的 SecondCommand 值（因为它是读写的）
                connection.SecondCommand = "SELECT * FROM Customers WHERE Country = 'USA'";
                Console.WriteLine("Updated SecondCommand value: " + connection.SecondCommand);
                
                // 清除 SecondCommand 以演示设置空字符串
                connection.SecondCommand = string.Empty;
                Console.WriteLine("Cleared SecondCommand value: " + connection.SecondCommand);
                
                // 使用修改后的连接设置保存工作簿
                workbook.Save("SecondCommandDemo.xlsx");
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

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


