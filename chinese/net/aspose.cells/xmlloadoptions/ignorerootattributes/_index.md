---
title: "XmlLoadOptions.IgnoreRootAttributes"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "XmlLoadOptions 属性。指示是否忽略根元素的属性"
type: docs
url: /zh/net/aspose.cells/xmlloadoptions/ignorerootattributes/
---
## XmlLoadOptions.IgnoreRootAttributes property

指示是否忽略根元素的属性。

```csharp
public bool IgnoreRootAttributes { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyIgnoreRootAttributesDemo
    {
        public static void Run()
        {
            // 创建 XML 加载选项并设置 IgnoreRootAttributes
            XmlLoadOptions options = new XmlLoadOptions();
            options.IgnoreRootAttributes = true;

            // 使用这些选项加载 XML 文件
            Workbook workbook = new Workbook("example.xml", options);

            // 访问已加载 XML 中的数据
            string cellValue = workbook.Worksheets[0].Cells["AH8"].StringValue;
            Console.WriteLine("Cell AH8 value: " + cellValue);

            // 另存为 XLSX
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


