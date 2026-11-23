---
title: "HtmlSaveOptions.CellNameAttribute"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "HtmlSaveOptions 属性。指定用于写入 CellName 的属性。例如，如果值为 id，则单元格 A1 的输出将为 td idA1。默认值为 null。"
type: docs
url: /zh/net/aspose.cells/htmlsaveoptions/cellnameattribute/
---
## HtmlSaveOptions.CellNameAttribute property

指定用于写入 CellName 的属性。（例如，如果值为 "id"，则单元格 "A1" 的输出将为:&lt;td id='A1'&gt;）。默认值为 null。

```csharp
public string CellNameAttribute { get; set; }
```

### 示例

```csharp
using System;
using System.IO;
using System.Text.RegularExpressions;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyCellNameAttributeDemo
    {
        public static void Run()
        {
            // 创建一个包含一些数据的示例工作簿。
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");
            worksheet.Cells["B2"].PutValue(123);

            // 使用 CellNameAttribute 设置 HTML 保存选项
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.CellNameAttribute = "id";
            saveOptions.ExportImagesAsBase64 = true;
            saveOptions.ExportActiveWorksheetOnly = true;

            // 保存为 HTML 文件
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);

            // 验证 HTML 输出包含单元格 ID
            string htmlContent = File.ReadAllText(outputPath);
            Console.WriteLine("HTML contains A1 cell with ID: " + Regex.IsMatch(htmlContent, @"<td\s+id='A1'"));
            Console.WriteLine("HTML contains B2 cell with ID: " + Regex.IsMatch(htmlContent, @"<td\s+id='B2'"));
        }
    }
}
```

### 另请参见

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


