---
title: "JsonSaveOptions.ExportHyperlinkType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "JsonSaveOptions 属性。表示导出超链接到 json 的类型"
type: docs
url: /zh/net/aspose.cells/jsonsaveoptions/exporthyperlinktype/
---
## JsonSaveOptions.ExportHyperlinkType property

表示导出超链接到 json 的类型。

```csharp
public JsonExportHyperlinkType ExportHyperlinkType { get; set; }
```

### 备注

默认值为 DisplayString；

### 示例

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Json;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportHyperlinkTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 向单元格 A1 添加超链接
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // 设置 JSON 的导出选项
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.HtmlString;
            
            // 将工作簿保存为 JSON
            string outputPath = "output.json";
            workbook.Save(outputPath, saveOptions);
            
            // 验证输出中包含超链接
            string jsonContent = File.ReadAllText(outputPath);
            Console.WriteLine("JSON content contains hyperlink: " + 
                jsonContent.Contains("https://www.aspose.com"));
        }
    }
}
```

### 另请参见

* enum [JsonExportHyperlinkType](../../../aspose.cells.json/jsonexporthyperlinktype/)
* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


