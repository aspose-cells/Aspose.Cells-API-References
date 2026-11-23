---
title: "CalculationOptions.CharacterEncoding"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "CalculationOptions 属性。指定在计算公式时用于字符编码/解码的编码方式。对于诸如 CHAR、CODE 等函数，计算结果取决于区域设置和环境的默认字符集。通过此属性，用户可以指定这些函数使用的正确编码，以获得预期的结果。"
type: docs
url: /zh/net/aspose.cells/calculationoptions/characterencoding/
---
## CalculationOptions.CharacterEncoding property

指定在计算公式时用于字符编码/解码的编码方式。对于诸如 CHAR、CODE 等函数，计算结果取决于区域设置和环境的默认字符集。通过此属性，用户可以指定这些函数使用的正确编码，以获得预期的结果。

```csharp
public Encoding CharacterEncoding { get; set; }
```

### 示例

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyCharacterEncodingDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            wb.Settings.Region = CountryCode.Japan;
            
            CalculationOptions copts = new CalculationOptions();
            copts.CharacterEncoding = Encoding.GetEncoding("iso-2022-jp");
            
            string formula = "=TRIM(1)";
            string result = (string)sheet.CalculateFormula(formula, copts);
            
            Console.WriteLine("Calculation result: " + result);
        }
    }
}
```

### 另请参见

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


