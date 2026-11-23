---
title: "DeleteBlankOptions.EmptyStringAsBlank"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "DeleteBlankOptions 属性。指示当单元格的值为空字符串时是否将其视为空白。默认值为 true"
type: docs
url: /zh/net/aspose.cells/deleteblankoptions/emptystringasblank/
---
## DeleteBlankOptions.EmptyStringAsBlank property

指示当单元格的值为空字符串时是否将其视为空白。默认值为 true。

```csharp
public bool EmptyStringAsBlank { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyEmptyStringAsBlankDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 填充工作表数据，包括空字符串
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue("");
            worksheet.Cells["A3"].PutValue("More Data");
            worksheet.Cells["A4"].PutValue("");
            worksheet.Cells["A5"].PutValue("Even More Data");

            // 将 DeleteBlankOptions 配置为 EmptyStringAsBlank 为 true
            DeleteBlankOptions options = new DeleteBlankOptions
            {
                EmptyStringAsBlank = true
            };

            // 删除包含空字符串的行（视为空白）
            worksheet.Cells.DeleteBlankRows(options);

            // 保存结果
            workbook.Save("DeleteBlankOptions_EmptyStringAsBlank_Output.xlsx");
        }
    }
}
```

### 另请参见

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


