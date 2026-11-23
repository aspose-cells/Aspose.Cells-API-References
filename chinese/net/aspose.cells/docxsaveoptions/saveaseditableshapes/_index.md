---
title: "DocxSaveOptions.SaveAsEditableShapes"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "DocxSaveOptions 属性。将所有绘图对象保存为 Word 文件中的可编辑形状，以便您可以在 Word 中编辑它们"
type: docs
url: /zh/net/aspose.cells/docxsaveoptions/saveaseditableshapes/
---
## DocxSaveOptions.SaveAsEditableShapes property

将所有绘图对象保存为 Word 文件中的可编辑形状，以便您可以在 Word 中编辑它们。

```csharp
public bool SaveAsEditableShapes { get; set; }
```

### 备注

仅适用于图表。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertySaveAsEditableShapesDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 访问第一个工作表并添加示例数据
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Editable Shapes Demo";

            try
            {
                // 初始化 DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // 显示 SaveAsEditableShapes 属性的默认值
                Console.WriteLine("Default SaveAsEditableShapes value: " + saveOptions.SaveAsEditableShapes);

                // 将 SaveAsEditableShapes 设置为 true 以演示其用法
                saveOptions.SaveAsEditableShapes = true;
                Console.WriteLine("SaveAsEditableShapes set to: " + saveOptions.SaveAsEditableShapes);

                // 使用配置的选项将工作簿保存为 DOCX
                workbook.Save("SaveAsEditableShapesDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with SaveAsEditableShapes option.");
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


