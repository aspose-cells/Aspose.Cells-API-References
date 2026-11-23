---
title: "DBConnection.ClassType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "DBConnection 属性。获取此 ExternalConnection 对象的类型"
type: docs
url: /zh/net/aspose.cells.externalconnections/dbconnection/classtype/
---
## DBConnection.ClassType property

获取此 [`ExternalConnection`](../../externalconnection/) 对象的类型。

```csharp
public override ExternalConnectionClassType ClassType { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertyClassTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            try
            {
                // 通过将其添加到集合中来创建新的 DBConnection 实例
                // 由于 DBConnection 没有公共的无参数构造函数，
                // 我们将让集合为我们创建它
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[connections.Count];
                
                // 显示 ClassType 值（只读属性）
                Console.WriteLine("DBConnection ClassType: " + dbConnection.ClassType);
                
                // 演示设置其他属性以使示例更具意义
                dbConnection.ConnectionString = "Server=myServerAddress;Database=myDataBase;";
                dbConnection.CommandType = OLEDBCommandType.TableName;
                dbConnection.Command = "Customers";
                
                // 保存工作簿
                workbook.Save("DBConnectionDemo.xlsx");
                
                Console.WriteLine("ClassType demonstration completed successfully.");
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

* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


