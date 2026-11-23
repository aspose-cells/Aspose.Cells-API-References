---
title: "Range.ToJson"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Range 方法。将范围转换为 JSON 值"
type: docs
url: /zh/net/aspose.cells/range/tojson/
---
## Range.ToJson method

将范围转换为 JSON 值。

```csharp
public string ToJson(JsonSaveOptions options)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| options | JsonSaveOptions | 转换的选项 |

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodToJsonWithJsonSaveOptionsDemo
    {
        public static void Run()
        {
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            
            // 示例数据
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Age");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["B2"].PutValue(30);

            Aspose.Cells.Range range = sheet.Cells.CreateRange("A1:B2");

            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.AlwaysExportAsJsonObject = true;
            saveOptions.ToExcelStruct = true;
            
            string json = range.ToJson(saveOptions);
            Console.WriteLine(json);
        }
    }
}
```

### 另请参见

* class [JsonSaveOptions](../../jsonsaveoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


