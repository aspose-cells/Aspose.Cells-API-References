---
title: "NumbersLoadOptions.NumbersLoadOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "NumbersLoadOptions 构造函数。构造函数"
type: docs
url: /zh/net/aspose.cells.numbers/numbersloadoptions/numbersloadoptions/
---
## NumbersLoadOptions constructor

构造函数。

```csharp
public NumbersLoadOptions()
```

### 示例

```csharp
using System;
using System.Globalization;
using Aspose.Cells;
using Aspose.Cells.Numbers;

namespace AsposeCellsExamples
{
    public class NumbersLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // 使用构造函数创建 NumbersLoadOptions
            NumbersLoadOptions loadOptions = new NumbersLoadOptions
            {
                // 设置一些常用属性
                Password = "secure123",
                ParsingFormulaOnOpen = true,
                CultureInfo = new CultureInfo("en-US"),
                StandardFont = "Arial",
                MemorySetting = MemorySetting.MemoryPreference
            };

            // 使用这些选项加载工作簿
            Workbook workbook = new Workbook("sample.numbers", loadOptions);

            // 另存为 XLSX
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [NumbersLoadOptions](../)
* namespace [Aspose.Cells.Numbers](../../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../../)


