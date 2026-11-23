---
title: "DBConnection.ConnectionString"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "DBConnection 属性。连接信息字符串用于与 OLE DB 或 ODBC 数据源建立联系"
type: docs
url: /zh/net/aspose.cells.externalconnections/dbconnection/connectionstring/
---
## DBConnection.ConnectionString property

连接信息字符串用于与 OLE DB 或 ODBC 数据源建立联系。

```csharp
public override string ConnectionString { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertyConnectionStringDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            try
            {
                // 访问外部连接的集合
                ExternalConnectionCollection connections = workbook.DataConnections;

                // 通过将其添加到集合中创建新的 DBConnection
                DBConnection dbConnection = (DBConnection)connections[connections.Count];

                // 显示初始 ConnectionString 值
                Console.WriteLine("Initial ConnectionString: " + dbConnection.ConnectionString);

                // 设置新的 ConnectionString
                dbConnection.ConnectionString = "Provider=Microsoft.Jet.OLEDB.4.0;Data Source=C:\\data\\database.mdb;";

                // 显示更新后的 ConnectionString 值
                Console.WriteLine("Updated ConnectionString: " + dbConnection.ConnectionString);

                // 保存工作簿
                workbook.Save("ConnectionStringDemo.xlsx");
                Console.WriteLine("ConnectionString demonstration completed successfully.");
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

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


