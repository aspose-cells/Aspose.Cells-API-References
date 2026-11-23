---
title: "LowCodeSplitOptions.SaveOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "LowCodeSplitOptions 属性。用于保存拆分部件的保存选项"
type: docs
url: /zh/net/aspose.cells.lowcode/lowcodesplitoptions/saveoptions/
---
## LowCodeSplitOptions.SaveOptions property

用于保存拆分后部分的保存选项。

```csharp
public LowCodeSaveOptions SaveOptions { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSplitOptionsPropertySaveOptionsDemo
    {
        public static void Run()
        {
            // 创建新工作簿并添加示例数据
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // 创建 LowCodeSplitOptions 的实例
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();

            // 显示初始 SaveOptions 值（默认 null）
            Console.WriteLine("Initial SaveOptions value: " + (splitOptions.SaveOptions == null ? "null" : splitOptions.SaveOptions.ToString()));

            // 为 PDF 格式创建并配置 LowCodeSaveOptions
            LowCodeSaveOptions pdfSaveOptions = new LowCodeSaveOptions();
            pdfSaveOptions.SaveFormat = SaveFormat.Pdf;

            // 将保存选项分配给 SplitOptions
            splitOptions.SaveOptions = pdfSaveOptions;

            // 显示更新后的 SaveOptions 值
            Console.WriteLine("Updated SaveOptions SaveFormat: " + splitOptions.SaveOptions.SaveFormat);

            // 示例使用场景：拆分工作簿会将部分保存为 PDF
            // (实际拆分代码取决于 Aspose.Cells.LowCode API 实现)
            // LowCodeEngine.Split(workbook, splitOptions, \"output_directory/\");
            
            // 保存原始工作簿以作演示（不受 SplitOptions 影响）
            workbook.Save("LowCodeSplitOptionsPropertySaveOptionsDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


