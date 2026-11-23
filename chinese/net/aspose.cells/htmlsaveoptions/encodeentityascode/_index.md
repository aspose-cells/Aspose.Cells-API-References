---
title: "HtmlSaveOptions.EncodeEntityAsCode"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "HtmlSaveOptions 属性。指示是否将 HTML 字符实体替换为十进制代码。例如，nbsp 将被替换为 160。默认值为 false"
type: docs
url: /zh/net/aspose.cells/htmlsaveoptions/encodeentityascode/
---
## HtmlSaveOptions.EncodeEntityAsCode property

指示是否将 HTML 字符实体替换为十进制代码。（例如，"&amp;nbsp;" 被替换为 "&amp;#160;"）。默认值为 false。

```csharp
public bool EncodeEntityAsCode { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class HtmlSaveOptionsPropertyEncodeEntityAsCodeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加带有特殊字符的示例数据
            worksheet.Cells["A1"].PutValue("Sample & Text");
            worksheet.Cells["A2"].PutValue("Another <Test> String");
            worksheet.Cells["A3"].PutValue("Price: $100");

            // 创建 HTML 保存选项
            HtmlSaveOptions options = new HtmlSaveOptions();

            // 显示 EncodeEntityAsCode 的当前值
            Console.WriteLine("Current EncodeEntityAsCode value: " + options.EncodeEntityAsCode);

            // 将 EncodeEntityAsCode 设置为 true
            options.EncodeEntityAsCode = true;

            // 以代码形式编码实体后保存
            workbook.Save("HtmlWithEncodedEntities.html", options);

            // 将 EncodeEntityAsCode 设置为 false
            options.EncodeEntityAsCode = false;

            // 以原样保存实体
            workbook.Save("HtmlWithRawEntities.html", options);

            // 比较输出文件
            Console.WriteLine("Files created:");
            Console.WriteLine("1. HtmlWithEncodedEntities.html - with encoded entities");
            Console.WriteLine("2. HtmlWithRawEntities.html - with raw entities");
        }
    }
}
```

### 另请参见

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


