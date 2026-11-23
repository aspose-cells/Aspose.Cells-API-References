---
title: "DataModelConnection.Command"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "DataModelConnection 属性。包含要传递给数据提供程序 API 的数据库命令字符串，该 API 将与外部源交互以检索数据"
type: docs
url: /zh/net/aspose.cells.externalconnections/datamodelconnection/command/
---
## DataModelConnection.Command property

包含要传递给数据提供程序 API 的数据库命令的字符串，该 API 将与外部源交互以检索数据

```csharp
public override string Command { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;
    using System.Runtime.Serialization;

    public class DataModelConnectionPropertyCommandDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            try
            {
                // 使用未初始化的对象创建 DataModelConnection 实例
                DataModelConnection connection = (DataModelConnection)FormatterServices.GetUninitializedObject(typeof(DataModelConnection));
                ((IList<ExternalConnection>)workbook.DataConnections).Add(connection);

                // 显示初始 Command 值（为空）
                Console.WriteLine("Initial Command: " + connection.Command);

                // 设置 Command 属性
                connection.Command = "SELECT * FROM Customers";
                
                // 显示更新后的 Command 值
                Console.WriteLine("Updated Command: " + connection.Command);

                // 为完整的连接设置其他必需的属性
                connection.CommandType = OLEDBCommandType.SqlStatement;
                connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";

                // 使用该连接保存工作簿
                workbook.Save("CommandDemo.xlsx");
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

* class [DataModelConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


