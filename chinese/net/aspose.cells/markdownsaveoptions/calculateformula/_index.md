---
title: "MarkdownSaveOptions.CalculateFormula"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "MarkdownSaveOptions 属性。指示是否在保存 markdown 文件之前计算公式"
type: docs
url: /zh/net/aspose.cells/markdownsaveoptions/calculateformula/
---
## MarkdownSaveOptions.CalculateFormula property

指示是否在保存 markdown 文件之前计算公式。

```csharp
public bool CalculateFormula { get; set; }
```

### 备注

默认值为 false。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyCalculateFormulaDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加包含公式的示例数据
            worksheet.Cells["A1"].PutValue("Price");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["C1"].PutValue("Total");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["C2"].Formula = "=A2*B2";

            try
            {
                // 创建 MarkdownSaveOptions 实例
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // 显示 CalculateFormula 的默认值
                Console.WriteLine("Default CalculateFormula value: " + saveOptions.CalculateFormula);

                // 将 CalculateFormula 设置为 true，以在保存前计算公式
                saveOptions.CalculateFormula = true;
                Console.WriteLine("CalculateFormula set to: " + saveOptions.CalculateFormula);

                // 在启用公式计算的情况下保存工作簿
                workbook.Save("CalculateFormula_Enabled.md", saveOptions);

                // 将 CalculateFormula 设置为 false，以原样保存公式
                saveOptions.CalculateFormula = false;
                Console.WriteLine("CalculateFormula set to: " + saveOptions.CalculateFormula);

                // 在禁用公式计算的情况下保存工作簿
                workbook.Save("CalculateFormula_Disabled.md", saveOptions);

                Console.WriteLine("CalculateFormula demonstration completed successfully.");
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


