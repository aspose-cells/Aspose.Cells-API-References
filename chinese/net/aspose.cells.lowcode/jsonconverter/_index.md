---
title: "类 JsonConverter"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.LowCode.JsonConverter 类。用于在 JSON 数据结构与其他电子表格文件格式之间转换的转换器"
type: docs
url: /zh/net/aspose.cells.lowcode/jsonconverter/
---
## JsonConverter class

用于在 JSON 数据结构与其他电子表格文件格式之间转换的转换器。

```csharp
public class JsonConverter
```

## 方法

| 名称 | 描述 |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/jsonconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | 在 JSON 数据与其他电子表格文件格式之间进行转换。 |
| static [Process](../../aspose.cells.lowcode/jsonconverter/process/#process_1)(string, string) | 在 JSON 与其他格式之间转换给定的模板文件。 |

### 示例

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassJsonConverterDemo
    {
        public static void Run()
        {
            string jsonFilePath = "data.json";
            string excelFilePath = "res.xlsx";

            try
            {
                // 使用 Aspose.Cells.LowCode.JsonConverter 将 JSON 转换为 Excel
                JsonConverter.Process(jsonFilePath, excelFilePath);

                Console.WriteLine("Conversion completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


