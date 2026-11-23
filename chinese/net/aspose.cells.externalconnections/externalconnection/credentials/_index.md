---
title: "ExternalConnection.Credentials"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ExternalConnection 属性。指定在建立或重新建立连接时使用的身份验证方法"
type: docs
url: /zh/net/aspose.cells.externalconnections/externalconnection/credentials/
---
## ExternalConnection.Credentials property

指定在建立（或重新建立）连接时使用的身份验证方法。

```csharp
[Obsolete("Use ExternalConnection.CredentialsMethodType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public CredentialsMethodType Credentials { get; set; }
```

### 备注

注意：此属性现已过时。请改用 ExternalConnection.CredentialsMethodType 属性。此属性将在自 2017 年 10 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyCredentialsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            try
            {
                // 访问第一个外部连接（假设存在）
                ExternalConnection connection = workbook.DataConnections[0];
                
                // 显示当前的 Credentials 值
                Console.WriteLine("Initial Credentials value: " + connection.Credentials);
                
                // 设置新的 Credentials 值（因为它是读写的）
                connection.Credentials = CredentialsMethodType.Integrated;
                Console.WriteLine("Updated Credentials value: " + connection.Credentials);
                
                // 循环遍历可能的值
                foreach (CredentialsMethodType method in Enum.GetValues(typeof(CredentialsMethodType)))
                {
                    connection.Credentials = method;
                    Console.WriteLine($"Credentials set to: {method}");
                }
                
                // 使用修改后的连接设置保存工作簿
                workbook.Save("CredentialsDemo.xlsx");
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

* enum [CredentialsMethodType](../../credentialsmethodtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


