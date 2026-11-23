---
title: "XmlLoadOptions.ConvertNumericOrDate"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "XmlLoadOptions 属性。指示是否将 XML 文件中的值转换为数字或日期"
type: docs
url: /zh/net/aspose.cells/xmlloadoptions/convertnumericordate/
---
## XmlLoadOptions.ConvertNumericOrDate property

指示是否将 XML 文件中的值转换为数字或日期。

```csharp
public bool ConvertNumericOrDate { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyConvertNumericOrDateDemo
    {
        public static void Run()
        {
            // 创建 XML 加载选项
            XmlLoadOptions options = new XmlLoadOptions();
            
            // 将 ConvertNumericOrDate 设置为 true（默认）
            options.ConvertNumericOrDate = true;
            Workbook wb1 = new Workbook("input.xml", options);
            Cell cell1 = wb1.Worksheets[0].Cells["A1"];
            Console.WriteLine("With conversion (true): " + cell1.Value + " is type: " + cell1.Type);
            
            // 将 ConvertNumericOrDate 设置为 false
            options.ConvertNumericOrDate = false;
            Workbook wb2 = new Workbook("input.xml", options);
            Cell cell2 = wb2.Worksheets[0].Cells["A1"];
            Console.WriteLine("Without conversion (false): " + cell2.Value + " is type: " + cell2.Type);
            
            // 保存结果
            wb1.Save("output_with_conversion.xlsx");
            wb2.Save("output_without_conversion.xlsx");
        }
    }
}
```

### 另请参见

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


