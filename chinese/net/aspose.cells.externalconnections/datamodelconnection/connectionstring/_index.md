---
title: "DataModelConnection.ConnectionString"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "DataModelConnection 属性。连接信息字符串用于与 OLE DB 或 ODBC 数据源建立联系"
type: docs
url: /zh/net/aspose.cells.externalconnections/datamodelconnection/connectionstring/
---
## DataModelConnection.ConnectionString property

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
    using System.Runtime.Serialization;

    public class DataModelConnectionPropertyConnectionStringDemo
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

                // 显示初始 ConnectionString 值（为空）
                Console.WriteLine("Initial ConnectionString: " + connection.ConnectionString);

                // 设置 ConnectionString 属性
                connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";
                
                // 显示更新后的 ConnectionString 值
                Console.WriteLine("Updated ConnectionString: " + connection.ConnectionString);

                // 为完整的连接设置其他必需的属性
                connection.Command = "SELECT * FROM Customers";
                connection.CommandType = OLEDBCommandType.SqlStatement;

                // 使用该连接保存工作簿
                workbook.Save("ConnectionStringDemo.xlsx");
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


