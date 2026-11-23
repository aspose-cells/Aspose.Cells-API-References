---
title: "JsonSaveOptions.AlwaysExportAsJsonObject"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "JsonSaveOptions 属性。指示是否始终将 Excel 导出为 JSON 对象，即使文件中只有一个工作表"
type: docs
url: /zh/net/aspose.cells/jsonsaveoptions/alwaysexportasjsonobject/
---
## JsonSaveOptions.AlwaysExportAsJsonObject property

指示是否始终将 Excel 导出为 JSON 对象，即使文件中只有一个工作表。

```csharp
public bool AlwaysExportAsJsonObject { get; set; }
```

### 示例

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyAlwaysExportAsJsonObjectDemo
    {
        public static void Run()
        {
            // 创建一个包含两个工作表的示例工作簿
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // 在第一个工作表中设置一些示例数据
            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Value");
            cells["A2"].PutValue("Item1");
            cells["B2"].PutValue(100);

            // 配置 JSON 保存选项
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.AlwaysExportAsJsonObject = true;
            saveOptions.ExportNestedStructure = true;
            saveOptions.SkipEmptyRows = true;

            // 保存为 JSON 文件
            string outputPath = "output.json";
            workbook.Save(outputPath, saveOptions);

            // 显示已保存的 JSON 内容
            string jsonContent = File.ReadAllText(outputPath);
            Console.WriteLine(jsonContent);
        }
    }
}
```

### 另请参见

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


