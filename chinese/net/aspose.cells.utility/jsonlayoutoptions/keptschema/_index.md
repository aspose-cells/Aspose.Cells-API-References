---
title: "JsonLayoutOptions.KeptSchema"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "JsonLayoutOptions 属性。指示是否保留此 json 的模式"
type: docs
url: /zh/net/aspose.cells.utility/jsonlayoutoptions/keptschema/
---
## JsonLayoutOptions.KeptSchema property

指示是否保留此 JSON 的模式。

```csharp
public bool KeptSchema { get; set; }
```

### 备注

有时我们会在加载 JSON 文件后将文件保存为 JSON。

### 示例

```csharp
using System;
using System.IO;
using System.Text.Json;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyKeptSchemaDemo
    {
        public class Data
        {
            public string RootProperty { get; set; }
            public Payload Payload { get; set; }
        }

        public class Payload
        {
            public ArrayData[] Array { get; set; }
            public string PayloadProperty { get; set; }
            public PayloadStruct PayloadStruct { get; set; }
        }

        public class ArrayData
        {
            public string ArrayProperty { get; set; }
        }

        public struct PayloadStruct
        {
            public string PayloadProperty1 { get; set; }
            public string PayloadProperty2 { get; set; }
        }

        public static void Run()
        {
            // 创建示例数据
            var data = new Data()
            {
                RootProperty = "RootValue",
                Payload = new Payload()
                {
                    Array = new[]
                    {
                        new ArrayData() { ArrayProperty = "item1" },
                        new ArrayData() { ArrayProperty = "item2" }
                    },
                    PayloadProperty = "PayloadValue",
                    PayloadStruct = new PayloadStruct()
                    {
                        PayloadProperty1 = "struct1",
                        PayloadProperty2 = "struct2"
                    }
                }
            };

            // 使用 System.Text.Json 将数据序列化为 JSON
            string json = JsonSerializer.Serialize(new[] { data });

            // 创建工作簿并导入 JSON
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            JsonLayoutOptions layoutOptions = new JsonLayoutOptions();
            layoutOptions.KeptSchema = true; // Demonstrate KeptSchema usage
            
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, layoutOptions);

            // 保存并输出结果
            string outputPath = "output/";
            Directory.CreateDirectory(outputPath);
            
            workbook.Save(outputPath + "KeptSchemaDemo.xlsx", SaveFormat.Xlsx);
            workbook.Save(outputPath + "KeptSchemaDemo.json", new JsonSaveOptions()
            {
                ExportNestedStructure = true
            });

            Console.WriteLine("Files saved successfully. Check output directory.");
        }
    }
}
```

### 另请参见

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


