---
title: "PaginatedSaveOptions.DefaultEditLanguage"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PaginatedSaveOptions 属性。获取或设置默认编辑语言"
type: docs
url: /zh/net/aspose.cells/paginatedsaveoptions/defaulteditlanguage/
---
## PaginatedSaveOptions.DefaultEditLanguage property

获取或设置默认编辑语言。

```csharp
public DefaultEditLanguage DefaultEditLanguage { get; set; }
```

### 备注

当设置不同的编辑语言时，文本段落可能会显示/渲染不同的布局。默认是 Auto。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyDefaultEditLanguageDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一些中日韩文本以演示 DefaultEditLanguage 属性
            worksheet.Cells["A1"].PutValue("日本語のテキスト");
            worksheet.Cells["A2"].PutValue("中文文本");
            worksheet.Cells["A3"].PutValue("한글 텍스트");

            // 创建 PDF 保存选项并将中日韩语言设为默认编辑语言
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.DefaultEditLanguage = DefaultEditLanguage.CJK;
            
            // 使用指定的选项保存工作簿
            workbook.Save("output.pdf", pdfSaveOptions);
            
            Console.WriteLine("Workbook saved with CJK as default edit language.");
        }
    }
}
```

### 另请参见

* enum [DefaultEditLanguage](../../defaulteditlanguage/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


