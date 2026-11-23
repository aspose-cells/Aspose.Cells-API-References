---
title: "WebQueryConnection.EditPage"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "WebQueryConnection 属性。显示 web query 数据的用户界面网页的 URL。如果 sourceDatatrue 为 true 且 url 已被重定向以引用 XML 文件，则该 URL 会被持久化。随后可以在 UI 中显示该用户界面页面，并在后台检索 XML 数据。"
type: docs
url: /zh/net/aspose.cells.externalconnections/webqueryconnection/editpage/
---
## WebQueryConnection.EditPage property

显示 web query 数据的用户面对网页的 URL。如果 sourceData=\"true\" 且 url 已被重定向以引用 XML 文件，则该 URL 会被持久化。随后可以在 UI 中显示该用户面对页面，并在后台检索 XML 数据。

```csharp
[Obsolete("Use WebQueryConnection.EditWebPage property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string EditPage { get; set; }
```

### 备注

注意：此属性现已废弃。请改用 WebQueryConnection.EditWebPage 属性。该属性将在自 2017 年 10 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyEditPageDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            try
            {
                // 如果可用，访问第一个现有的 web query 连接
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // 显示初始 EditPage 值
                    Console.WriteLine("Initial EditPage value: " + connection.EditPage);
                    
                    // 将 EditPage 设置为新 URL（因为它是读写的）
                    connection.EditPage = "https://example.com/editpage";
                    Console.WriteLine("Updated EditPage value: " + connection.EditPage);
                    
                    // 保存工作簿
                    workbook.Save("WebQueryConnectionEditPageDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connection found in the workbook.");
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

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


