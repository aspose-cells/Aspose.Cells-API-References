---
title: "DocxSaveOptions.SaveAsEditableShaps"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "DocxSaveOptions 属性。将所有绘图对象保存为 Word 文件中的可编辑形状。这样您就可以在 Word 中编辑它们"
type: docs
url: /zh/net/aspose.cells/docxsaveoptions/saveaseditableshaps/
---
## DocxSaveOptions.SaveAsEditableShaps property

将所有绘图对象保存为 Word 文件中的可编辑形状。这样您就可以在 Word 中编辑它们。

```csharp
[Obsolete("Use SaveFormat.SaveAsEditableShapes instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SaveAsEditableShaps { get; set; }
```

### 备注

注意：此成员现已过时。请改用 [`SaveAsEditableShapes`](../saveaseditableshapes/) 属性。该属性将在自 2025 年 5 月起 6 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsPropertySaveAsEditableShapsDemo
    {
        public static void Run()
        {
            // 创建一个工作簿对象并打开模板 Excel 文件
            Workbook workbook = new Workbook("example.xlsx");

            // 初始化 DocxSaveOptions
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            
            // 将 SaveAsEditableShaps 属性设置为 true
            saveOptions.SaveAsEditableShaps = true;

            // 使用指定的选项将工作簿保存为 DOCX
            workbook.Save("example.docx", saveOptions);
        }
    }
}
```

### 另请参见

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


