---
title: "PptxSaveOptions.IgnoreHiddenRows"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PptxSaveOptions 属性。指示在将 Excel 转换为 PowerPoint 时是否忽略隐藏的行"
type: docs
url: /zh/net/aspose.cells/pptxsaveoptions/ignorehiddenrows/
---
## PptxSaveOptions.IgnoreHiddenRows property

指示在将 Excel 转换为 PowerPoint 时是否忽略隐藏的行。

```csharp
public bool IgnoreHiddenRows { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsPropertyIgnoreHiddenRowsDemo
    {
        public static void Run()
        {
            // 使用示例数据创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 添加示例数据并隐藏某些行
            worksheet.Cells["A1"].PutValue("Visible Row 1");
            worksheet.Cells["A2"].PutValue("Hidden Row");
            worksheet.Cells["A3"].PutValue("Visible Row 2");
            
            // 隐藏第 2 行
            worksheet.Cells.Rows[1].IsHidden = true;

            // 使用 IgnoreHiddenRows 设置 PPTX 保存选项
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.IgnoreHiddenRows = true;
            
            // 另存为 PPTX
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("PPTX saved with hidden rows ignored.");
        }
    }
}
```

### 另请参见

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


