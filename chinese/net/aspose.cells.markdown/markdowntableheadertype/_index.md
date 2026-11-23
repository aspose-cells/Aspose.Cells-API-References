---
title: "枚举 MarkdownTableHeaderType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Markdown.MarkdownTableHeaderType 枚举。表示 markdown 文件中表格的标题类型"
type: docs
url: /zh/net/aspose.cells.markdown/markdowntableheadertype/
---
## MarkdownTableHeaderType enumeration

表示 markdown 文件中表格的标题类型。

```csharp
public enum MarkdownTableHeaderType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| FirstRow | `0` | 第一行作为表格的标题。 |
| ColumnHeader | `1` | 列名（例如 A、B、C...）作为表格的标题。 |
| Empty | `2` | 一个空的标题行。 |

### 示例

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Markdown;

namespace AsposeCellsExamples
{
    public class MarkdownClassMarkdownTableHeaderTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 向单元格添加示例数据
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");

            // 设置 Markdown 保存选项
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.TableHeaderType = MarkdownTableHeaderType.FirstRow;
            
            // 另存为 Markdown 文件
            workbook.Save("output.md", saveOptions);
            
            // 验证输出
            string text = File.ReadAllText("output.md");
            Console.WriteLine(text.Contains("---|") ? "Success" : "Failed");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Markdown](../../aspose.cells.markdown/)
* assembly [Aspose.Cells](../../)


