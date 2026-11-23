---
title: "LowCodeHtmlSaveOptions.HtmlOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "LowCodeHtmlSaveOptions 属性。保存 HTML 的通用选项。"
type: docs
url: /zh/net/aspose.cells.lowcode/lowcodehtmlsaveoptions/htmloptions/
---
## LowCodeHtmlSaveOptions.HtmlOptions property

保存 HTML 的通用选项。

```csharp
public HtmlSaveOptions HtmlOptions { get; set; }
```

### 备注

当指定一个 [`HtmlSaveOptions`](../../../aspose.cells/htmlsaveoptions/) 实例时，[`SaveFormat`](../saveformat/) 将被覆盖（如果之前已指定）。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeHtmlSaveOptionsPropertyHtmlOptionsDemo
    {
        public static void Run()
        {
            // 使用示例数据创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.99);
            
            // 创建低代码 HTML 保存选项
            LowCodeHtmlSaveOptions saveOptions = new LowCodeHtmlSaveOptions
            {
                SaveFormat = SaveFormat.Html,
                HtmlOptions = new HtmlSaveOptions()
            };

            // 显示当前网格线导出设置
            Console.WriteLine("Export gridlines initially: " + saveOptions.HtmlOptions.ExportGridLines);

            // 保存时显示网格线
            workbook.Save("HtmlWithGridlines.html", saveOptions.HtmlOptions);

            // 修改 HTML 选项以隐藏网格线
            saveOptions.HtmlOptions = new HtmlSaveOptions { ExportGridLines = false };
            Console.WriteLine("Export gridlines after modification: " + saveOptions.HtmlOptions.ExportGridLines);

            // 保存时不显示网格线
            workbook.Save("HtmlWithoutGridlines.html", saveOptions.HtmlOptions);

            Console.WriteLine("Demo executed successfully. Compare output files.");
        }
    }
}
```

### 另请参见

* class [HtmlSaveOptions](../../../aspose.cells/htmlsaveoptions/)
* class [LowCodeHtmlSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


