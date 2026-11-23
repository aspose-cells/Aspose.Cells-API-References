---
title: "MarkdownSaveOptions.SplitTablesByBlankRow"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "MarkdownSaveOptions 属性。指示在导出为 Markdown 时，工作表中的空行是否应被视为表格分隔符。默认值为 false"
type: docs
url: /zh/net/aspose.cells/markdownsaveoptions/splittablesbyblankrow/
---
## MarkdownSaveOptions.SplitTablesByBlankRow property

指示在导出为 Markdown 时，工作表中的空行是否应被视为表格分隔符。默认值为 false。

```csharp
public bool SplitTablesByBlankRow { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertySplitTablesByBlankRowDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加包含空行的示例数据以演示表格拆分
            worksheet.Cells["A1"].Value = "Table 1 Header";
            worksheet.Cells["B1"].Value = "Value 1";
            worksheet.Cells["A2"].Value = "Data 1";
            worksheet.Cells["B2"].Value = "Data 2";

            // 添加一行空行（第 3 行）
            worksheet.Cells["A4"].Value = "Table 2 Header";
            worksheet.Cells["B4"].Value = "Value 2";
            worksheet.Cells["A5"].Value = "Data 3";
            worksheet.Cells["B5"].Value = "Data 4";

            // 创建 MarkdownSaveOptions 实例
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            try
            {
                // 显示默认的 SplitTablesByBlankRow 值
                Console.WriteLine("Default SplitTablesByBlankRow value: " +
                    saveOptions.SplitTablesByBlankRow);

                // 将 SplitTablesByBlankRow 设置为 true，以通过空行拆分表格
                saveOptions.SplitTablesByBlankRow = true;

                // 显示更新后的值
                Console.WriteLine("Updated SplitTablesByBlankRow value: " +
                    saveOptions.SplitTablesByBlankRow);

                // 将工作簿保存为启用表格拆分的 markdown
                workbook.Save("SplitTablesByBlankRowDemo.md", saveOptions);
                Console.WriteLine("Markdown file saved with table splitting by blank rows enabled.");
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

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


