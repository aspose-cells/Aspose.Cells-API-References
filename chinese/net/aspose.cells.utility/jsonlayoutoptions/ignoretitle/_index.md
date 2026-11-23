---
title: "JsonLayoutOptions.IgnoreTitle"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "JsonLayoutOptions 属性。忽略属性的标题"
type: docs
url: /zh/net/aspose.cells.utility/jsonlayoutoptions/ignoretitle/
---
## JsonLayoutOptions.IgnoreTitle property

忽略属性的标题

```csharp
public bool IgnoreTitle { get; set; }
```

### 示例

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyIgnoreTitleDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 示例 JSON 数据
            string jsonInput = @"{
                ""Products"": [
                    {
                        ""Name"": ""Product1"",
                        ""Price"": 100,
                        ""Date"": ""2023-01-15""
                    },
                    {
                        ""Name"": ""Product2"",
                        ""Price"": 200,
                        ""Date"": ""2023-02-20""
                    }
                ]
            }";

            // 将 JsonLayoutOptions 的 IgnoreTitle 设置为 true
            JsonLayoutOptions options = new JsonLayoutOptions();
            options.IgnoreTitle = true;  // This will skip the title row in output
            options.ArrayAsTable = true;
            options.DateFormat = "yyyy/MM/dd";

            // 导入 JSON 数据
            JsonUtility.ImportData(jsonInput, worksheet.Cells, 0, 0, options);

            // 保存工作簿
            workbook.Save("output_ignore_title.xlsx");
        }
    }
}
```

### 另请参见

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


