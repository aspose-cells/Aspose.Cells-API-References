---
title: "MarkdownLoadOptions.HasFormula"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "MarkdownLoadOptions 属性。指示如果文本以... 开头则为公式"
type: docs
url: /zh/net/aspose.cells/markdownloadoptions/hasformula/
---
## MarkdownLoadOptions.HasFormula property

指示文本是否为公式（如果以 "=" 开头）。

```csharp
public bool HasFormula { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownLoadOptionsPropertyHasFormulaDemo
    {
        public static void Run()
        {
            try
            {
                // 创建 MarkdownLoadOptions 的实例
                MarkdownLoadOptions options = new MarkdownLoadOptions();

                // 显示 HasFormula 的默认值
                Console.WriteLine($"Default HasFormula value: {options.HasFormula}");

                // 将 HasFormula 设置为 true
                options.HasFormula = true;
                Console.WriteLine($"HasFormula set to: {options.HasFormula}");

                // 将 HasFormula 设置为 false
                options.HasFormula = false;
                Console.WriteLine($"HasFormula set to: {options.HasFormula}");

                // 创建一个包含示例 markdown 内容的工作簿
                Workbook workbook = new Workbook();

                // 保存工作簿以演示可以使用这些选项
                workbook.Save("HasFormulaDemo.xlsx");

                Console.WriteLine("HasFormula property demonstration completed successfully.");
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

* class [MarkdownLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


