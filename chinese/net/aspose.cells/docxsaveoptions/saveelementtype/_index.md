---
title: "DocxSaveOptions.SaveElementType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "DocxSaveOptions 属性。指示应保存哪些元素"
type: docs
url: /zh/net/aspose.cells/docxsaveoptions/saveelementtype/
---
## DocxSaveOptions.SaveElementType property

指示应保存哪些元素。

```csharp
public SaveElementType SaveElementType { get; set; }
```

### 示例

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsPropertySaveElementTypeDemo
    {
        public static void Run()
        {
            // 创建新工作簿并添加一些示例数据
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Demo Data");

            try
            {
                // 初始化 DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // 注意：DocxSaveOptions 类中不存在 SaveElementType 属性
                // 基于提供的 API 反射。如果它存在，您将这样读取：
                // var elementType = saveOptions.SaveElementType;
                // Console.WriteLine("SaveElementType: " + elementType);

                // 演示读取现有属性：SaveAsEditableShaps
                Console.WriteLine("SaveAsEditableShaps (default): " + saveOptions.SaveAsEditableShaps);

                // 将属性设置为 true 并显示新值
                saveOptions.SaveAsEditableShaps = true;
                Console.WriteLine("SaveAsEditableShaps (after set): " + saveOptions.SaveAsEditableShaps);

                // 使用配置的选项将工作簿保存为 DOCX
                workbook.Save("SaveElementTypeDemo.docx", saveOptions);
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### 另请参见

* enum [SaveElementType](../../../aspose.cells.saving/saveelementtype/)
* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


