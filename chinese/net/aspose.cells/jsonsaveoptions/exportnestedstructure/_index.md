---
title: "JsonSaveOptions.ExportNestedStructure"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "JsonSaveOptions 属性。导出为父子层次的 Json 结构"
type: docs
url: /zh/net/aspose.cells/jsonsaveoptions/exportnestedstructure/
---
## JsonSaveOptions.ExportNestedStructure property

导出为父子层次的 Json 结构。

```csharp
public bool ExportNestedStructure { get; set; }
```

### 示例

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportNestedStructureDemo
    {
        public static void Run()
        {
            // 创建一个包含嵌套数据的示例工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 创建嵌套数据结构
            worksheet.Cells["A1"].PutValue("Parent");
            worksheet.Cells["B1"].PutValue("Child");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Fruits");
            worksheet.Cells["B3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Vegetables");
            worksheet.Cells["B4"].PutValue("Carrot");

            // 使用 ExportNestedStructure 配置 JSON 保存选项
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.ExportNestedStructure = true;
            saveOptions.AlwaysExportAsJsonObject = true;

            // 以嵌套结构保存
            string outputPath = "output_nested.json";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("Workbook exported to JSON with nested structure. Output: " + outputPath);
        }
    }
}
```

### 另请参见

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


