---
title: "JsonSaveOptions.SkipEmptyRows"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "JsonSaveOptions 属性。指示是否跳过空行"
type: docs
url: /zh/net/aspose.cells/jsonsaveoptions/skipemptyrows/
---
## JsonSaveOptions.SkipEmptyRows property

指示是否跳过空行。

```csharp
public bool SkipEmptyRows { get; set; }
```

### 示例

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertySkipEmptyRowsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 示例数据 - 添加一些带值的单元格并让某些行保持为空
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            // 将第 3 行留空
            worksheet.Cells["A4"].PutValue("Data3");
            worksheet.Cells["B4"].PutValue("Data4");

            // 使用 SkipEmptyRows 配置 JSON 保存选项
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.SkipEmptyRows = true; // This will skip the empty row 3
            
            // 保存为 JSON
            string outputPath = "output.json";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("JSON saved with SkipEmptyRows=true. Empty rows were skipped.");
        }
    }
}
```

### 另请参见

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


