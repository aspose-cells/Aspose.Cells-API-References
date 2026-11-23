---
title: "DocxSaveOptions.AsNormalView"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "DocxSaveOptions 属性。将 Excel 文件导出为普通视图的 docx 文件。如果此属性为 true，将输出一个区域且不进行缩放。默认值为 false"
type: docs
url: /zh/net/aspose.cells/docxsaveoptions/asnormalview/
---
## DocxSaveOptions.AsNormalView property

将 Excel 文件导出为普通视图的 docx 文件。如果此属性为 true，将输出一个区域且不进行缩放。默认值为 false。

```csharp
public bool AsNormalView { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertyAsNormalViewDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 访问第一个工作表并添加示例数据
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Normal View Demo";

            try
            {
                // 初始化 DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // 显示 AsNormalView 属性的默认值
                Console.WriteLine("Default AsNormalView value: " + saveOptions.AsNormalView);

                // 将 AsNormalView 设置为 true 以演示其用法
                saveOptions.AsNormalView = true;
                Console.WriteLine("AsNormalView set to: " + saveOptions.AsNormalView);

                // 使用配置的选项将工作簿保存为 DOCX
                workbook.Save("AsNormalViewDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with AsNormalView option.");
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


