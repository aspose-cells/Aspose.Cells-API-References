---
title: "DocxSaveOptions.AsFlatOpc"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "DocxSaveOptions 属性。指示是否保存为可由 Open XML SDK 生成的平面 opc 文件"
type: docs
url: /zh/net/aspose.cells/docxsaveoptions/asflatopc/
---
## DocxSaveOptions.AsFlatOpc property

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

    public class DocxSaveOptionsPropertyAsFlatOpcDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 访问第一个工作表并添加示例数据
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Flat OPC Demo";

            try
            {
                // 初始化 DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // 显示 AsFlatOpc 属性的默认值
                Console.WriteLine("Default AsFlatOpc value: " + saveOptions.AsFlatOpc);

                // 将 AsFlatOpc 设置为 true 以演示其用法
                saveOptions.AsFlatOpc = true;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions.AsFlatOpc);

                // 使用配置的选项将工作簿保存为 DOCX
                workbook.Save("AsFlatOpcDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with AsFlatOpc option.");
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

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


