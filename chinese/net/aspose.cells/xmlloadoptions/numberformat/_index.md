---
title: "XmlLoadOptions.NumberFormat"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "XmlLoadOptions 属性。获取和设置数值的格式"
type: docs
url: /zh/net/aspose.cells/xmlloadoptions/numberformat/
---
## XmlLoadOptions.NumberFormat property

获取和设置数值的格式。

```csharp
public string NumberFormat { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyNumberFormatDemo
    {
        public static void Run()
        {
            // 创建 XmlLoadOptions 的实例
            XmlLoadOptions options = new XmlLoadOptions();

            // 将 NumberFormat 属性设置为显示两位小数的数字
            options.NumberFormat = "0.00";

            // 使用指定的选项将 XML 文件加载到工作簿中
            Workbook workbook = new Workbook("input.xml", options);

            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];

            // 设置一些数值以演示数字格式化
            worksheet.Cells["A1"].PutValue(123);
            worksheet.Cells["A2"].PutValue(45.678);
            worksheet.Cells["A3"].PutValue(0.5);

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


