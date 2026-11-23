---
title: "JsonConverter.Process"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "JsonConverter 方法。将给定的模板文件在 JSON 和其他格式之间转换"
type: docs
url: /zh/net/aspose.cells.lowcode/jsonconverter/process/
---
## Process(string, string) {#process_1}

在 JSON 与其他格式之间转换给定的模板文件。

```csharp
public static void Process(string templateFile, string resultFile)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| templateFile | String | 待转换的模板文件 |
| resultFile | String | 生成的文件 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class JsonConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            // 创建示例 JSON 数据并写入临时文件
            string jsonData = "{\"employees\":[{\"name\":\"John\", \"department\":\"Sales\"}, {\"name\":\"Jane\", \"department\":\"Marketing\"}]}";
            string templatePath = "template.json";
            File.WriteAllText(templatePath, jsonData);

            string resultPath = "output.xlsx";

            try
            {
                // 使用 JsonConverter 的静态方法直接处理文件
                JsonConverter.Process(templatePath, resultPath);

                Console.WriteLine($"Successfully converted JSON to spreadsheet. Output: {resultPath}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Conversion error: {ex.Message}");
            }
            finally
            {
                // 清理临时 JSON 文件
                if (File.Exists(templatePath))
                {
                    File.Delete(templatePath);
                }
            }
        }
    }
}
```

### 另请参见

* class [JsonConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

在 JSON 数据与其他电子表格文件格式之间进行转换。

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | 输入和加载的选项 |
| saveOptions | LowCodeSaveOptions | 输出和保存的选项 |

### 示例

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class JsonConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            // 创建示例 JSON 数据
            string jsonData = "{\"name\":\"John\", \"age\":30, \"city\":\"New York\"}";
            
            // 使用 JSON 数据创建内存流
            using (MemoryStream stream = new MemoryStream(System.Text.Encoding.UTF8.GetBytes(jsonData)))
            {
                // 使用 LowCode 选项处理 JSON 数据
                JsonConverter.Process(
                    new LowCodeLoadOptions() { InputStream = stream },
                    new LowCodeSaveOptions()
                    {
                        OutputFile = "output.json"
                    });
            }

            Console.WriteLine("JSON processing completed successfully.");
        }
    }
}
```

### 另请参见

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [JsonConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


