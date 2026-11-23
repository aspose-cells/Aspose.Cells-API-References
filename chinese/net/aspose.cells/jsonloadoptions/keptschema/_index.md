---
title: "JsonLoadOptions.KeptSchema"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "JsonLoadOptions 属性。指示是否保留此 JSON 的模式"
type: docs
url: /zh/net/aspose.cells/jsonloadoptions/keptschema/
---
## JsonLoadOptions.KeptSchema property

指示是否保留此 JSON 的模式。

```csharp
public bool KeptSchema { get; set; }
```

### 备注

有时我们会在加载 JSON 文件后将文件保存为 JSON。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class JsonLoadOptionsPropertyKeptSchemaDemo
    {
        public static void Run()
        {
            // 创建 JSON 加载选项
            JsonLoadOptions options = new JsonLoadOptions();

            // 显示 KeptSchema 属性的默认值
            Console.WriteLine("Default KeptSchema value: " + options.KeptSchema);

            // 将 KeptSchema 设置为 true
            options.KeptSchema = true;
            Console.WriteLine("KeptSchema set to: " + options.KeptSchema);

            // 创建示例 JSON 文件
            string jsonData = @"{
                ""Employees"": [
                    { ""ID"": 1, ""Name"": ""John"", ""Department"": ""Sales"" },
                    { ""ID"": 2, ""Name"": ""Jane"", ""Department"": ""Marketing"" }
                ]
            }";

            System.IO.File.WriteAllText("sample.json", jsonData);

            try
            {
                // 在启用 KeptSchema 的情况下加载 JSON
                Workbook workbook = new Workbook("sample.json", options);

                // 显示已加载工作簿的信息
                Console.WriteLine("Workbook loaded with KeptSchema: " + options.KeptSchema);
                Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);

                // 保存工作簿
                workbook.Save("KeptSchemaOutput.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


