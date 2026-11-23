---
title: "PaginatedSaveOptions.CheckFontCompatibility"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PaginatedSaveOptions 属性。指示是否对文本中的每个字符检查字体兼容性"
type: docs
url: /zh/net/aspose.cells/paginatedsaveoptions/checkfontcompatibility/
---
## PaginatedSaveOptions.CheckFontCompatibility property

指示是否检查文本中每个字符的字体兼容性。

```csharp
public bool CheckFontCompatibility { get; set; }
```

### 备注

默认值为 true。禁用此属性可能会提升性能。但当默认或指定的文本/字符字体无法用于渲染时，生成的 PDF 可能会出现不可读的字符（例如方块）。在这种情况下，用户应保持此属性为 true，以便搜索并使用替代字体来渲染文本。;

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyCheckFontCompatibilityDemo
    {
        public static void Run()
        {
            // 创建包含示例数据的新工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Font Compatibility Test");

            // 创建分页保存选项
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // 演示 CheckFontCompatibility 属性
            saveOptions.CheckFontCompatibility = false; // Disable font compatibility checking
            
            // 设置其他必需的属性
            saveOptions.DefaultFont = "Arial";
            saveOptions.CheckWorkbookDefaultFont = true;

            // 使用指定的选项保存文档
            workbook.Save("PaginatedSaveOptions_CheckFontCompatibility.pdf", saveOptions);
            
            Console.WriteLine("Document saved with CheckFontCompatibility = false");
        }
    }
}
```

### 另请参见

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


