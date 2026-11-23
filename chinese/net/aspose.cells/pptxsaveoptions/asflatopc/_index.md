---
title: "PptxSaveOptions.AsFlatOpc"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PptxSaveOptions 属性。指示是否将保存为可由 Open XML SDK 生成的平面 OPC 文件"
type: docs
url: /zh/net/aspose.cells/pptxsaveoptions/asflatopc/
---
## PptxSaveOptions.AsFlatOpc property

指示是否保存为可由 Open XML SDK 生成的平面 opc 文件

```csharp
public bool AsFlatOpc { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PptxSaveOptionsPropertyAsFlatOpcDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 创建示例工作表
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一些数据以使示例更有意义
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = "Flat OPC Demo";

            try
            {
                // 创建 PptxSaveOptions 实例
                PptxSaveOptions saveOptions = new PptxSaveOptions();

                // 显示 AsFlatOpc 的默认值
                Console.WriteLine("Default AsFlatOpc value: " + saveOptions.AsFlatOpc);

                // 将属性设置为 true 以演示其用法
                saveOptions.AsFlatOpc = true;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions.AsFlatOpc);

                // 在启用该选项的情况下将工作簿保存为 PPTX
                workbook.Save("AsFlatOpcDemo.pptx", saveOptions);

                Console.WriteLine("PPTX saved with AsFlatOpc enabled");
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

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


