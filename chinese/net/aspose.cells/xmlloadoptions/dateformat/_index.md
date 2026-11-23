---
title: "XmlLoadOptions.DateFormat"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "XmlLoadOptions 属性。获取和设置日期值的格式"
type: docs
url: /zh/net/aspose.cells/xmlloadoptions/dateformat/
---
## XmlLoadOptions.DateFormat property

获取和设置日期值的格式。

```csharp
public string DateFormat { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyDateFormatDemo
    {
        public static void Run()
        {
            // 创建 XmlLoadOptions 的实例
            XmlLoadOptions options = new XmlLoadOptions();

            // 设置用于从 XML 解析日期的日期格式
            options.DateFormat = "yyyy-MM-dd";
            options.ConvertNumericOrDate = true;

            // 使用指定的选项将 XML 文件加载到工作簿中
            Workbook workbook = new Workbook("input.xml", options);

            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];

            // 显示一些单元格以演示日期格式化
            Console.WriteLine("Cell A1: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("Cell A2: " + worksheet.Cells["A2"].Value);

            // 将工作簿保存到新文件
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


