---
title: "OoxmlSaveOptions.AsFlatOpc"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "OoxmlSaveOptions 属性。指示是否保存为可以由 Open XML SDK 生成的平面 opc 文件"
type: docs
url: /zh/net/aspose.cells/ooxmlsaveoptions/asflatopc/
---
## OoxmlSaveOptions.AsFlatOpc property

指示是否保存为可以由 Open XML SDK 生成的平面 opc 文件。

```csharp
public bool AsFlatOpc { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlSaveOptionsPropertyAsFlatOpcDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一些数据以使示例更有意义
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("Flat OPC Demo");

            try
            {
                // 创建 OoxmlSaveOptions 实例
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();

                // 显示 AsFlatOpc 属性的默认值
                Console.WriteLine("Default AsFlatOpc value: " + saveOptions.AsFlatOpc);

                // 将 AsFlatOpc 设置为 true
                saveOptions.AsFlatOpc = true;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions.AsFlatOpc);

                // 保存工作簿时启用 AsFlatOpc
                workbook.Save("AsFlatOpc_Enabled.xlsx", saveOptions);

                // 创建另一个 AsFlatOpc 已禁用的保存选项
                OoxmlSaveOptions saveOptions2 = new OoxmlSaveOptions();
                saveOptions2.AsFlatOpc = false;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions2.AsFlatOpc);

                // 保存工作簿时禁用 AsFlatOpc
                workbook.Save("AsFlatOpc_Disabled.xlsx", saveOptions2);

                Console.WriteLine("AsFlatOpc property demonstration completed successfully.");
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

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


