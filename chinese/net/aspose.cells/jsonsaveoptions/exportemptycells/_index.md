---
title: "JsonSaveOptions.ExportEmptyCells"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "JsonSaveOptions 属性。指示是否将空单元格导出为 null"
type: docs
url: /zh/net/aspose.cells/jsonsaveoptions/exportemptycells/
---
## JsonSaveOptions.ExportEmptyCells property

指示是否将空单元格导出为 null。

```csharp
public bool ExportEmptyCells { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportEmptyCellsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 填充包含一些空单元格的数据
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B3"].PutValue(2.99); // B2 is intentionally left empty

            // 创建 JsonSaveOptions 并将 ExportEmptyCells 设置为 false
            JsonSaveOptions options = new JsonSaveOptions
            {
                ExportEmptyCells = false
            };

            // 保存为 JSON - 空单元格将被跳过
            workbook.Save("output_skip_empty.json", options);

            // 将 ExportEmptyCells 更改为 true
            options.ExportEmptyCells = true;

            // 再次保存 - 空单元格将被包含
            workbook.Save("output_include_empty.json", options);
        }
    }
}
```

### 另请参见

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


