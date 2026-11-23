---
title: "枚举 JsonExportHyperlinkType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Json.JsonExportHyperlinkType 枚举。表示导出超链接到 json 的方式"
type: docs
url: /zh/net/aspose.cells.json/jsonexporthyperlinktype/
---
## JsonExportHyperlinkType enumeration

表示导出超链接到 JSON 的类型。

```csharp
public enum JsonExportHyperlinkType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| DisplayString | `0` | 导出显示字符串 |
| Address | `1` | 导出 URL |
| HtmlString | `2` | 导出为 HTML 字符串。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Json;
    using System;

    public class JsonExportHyperlinkTypeDemo
    {
        public static void JsonExportHyperlinkTypeExample()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一些带有超链接的示例数据
            worksheet.Cells["A1"].PutValue("Google");
            worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.google.com");

            worksheet.Cells["A2"].PutValue("Aspose");
            worksheet.Hyperlinks.Add("A2", 1, 1, "http://www.aspose.com");

            // 创建 JsonSaveOptions 并设置 ExportHyperlinkType
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.DisplayString;

            // 将工作簿保存为 JSON 格式
            workbook.Save("JsonExportHyperlinkTypeExample_HyperlinksDisplayString.json", saveOptions);

            // 将 ExportHyperlinkType 更改为 Address 并再次保存
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.Address;
            workbook.Save("JsonExportHyperlinkTypeExample_HyperlinksAddress.json", saveOptions);

            // 将 ExportHyperlinkType 更改为 HtmlString 并再次保存
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.HtmlString;
            workbook.Save("JsonExportHyperlinkTypeExample_HyperlinksHtmlString.json", saveOptions);

            Console.WriteLine("Workbooks saved with different hyperlink export types.");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Json](../../aspose.cells.json/)
* assembly [Aspose.Cells](../../)


