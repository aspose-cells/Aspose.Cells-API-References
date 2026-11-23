---
title: "WebQueryConnection.ClassType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "WebQueryConnection 属性。获取此 ExternalConnection 对象的类型"
type: docs
url: /zh/net/aspose.cells.externalconnections/webqueryconnection/classtype/
---
## WebQueryConnection.ClassType property

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

    public class WebQueryConnectionPropertyClassTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            try
            {
                // 访问现有的 web query 连接，或通过适当的初始化创建一个
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // 显示 ClassType 值（只读属性）
                    Console.WriteLine("WebQueryConnection ClassType: " + connection.ClassType);
                    
                    // 验证 web query 的预期枚举值
                    Console.WriteLine("Expected WebQuery enum value: " + 
                        (connection.ClassType == ExternalConnectionClassType.WebQuery ? "Match" : "Mismatch"));
                    
                    // 保存工作簿
                    workbook.Save("WebQueryConnectionClassTypeDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connections found in the workbook.");
                }
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
* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


