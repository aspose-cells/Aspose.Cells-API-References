---
title: "NumbersLoadOptions.LoadTableType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "NumbersLoadOptions 属性。获取和设置在同一工作表中加载多个表的类型"
type: docs
url: /zh/net/aspose.cells.numbers/numbersloadoptions/loadtabletype/
---
## NumbersLoadOptions.LoadTableType property

获取和设置在一个工作表中加载多个表的类型。

```csharp
public LoadNumbersTableType LoadTableType { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Numbers;

namespace AsposeCellsExamples
{
    public class NumbersLoadOptionsPropertyLoadTableTypeDemo
    {
        public static void Run()
        {
            // 创建 NumbersLoadOptions 的实例
            NumbersLoadOptions loadOptions = new NumbersLoadOptions
            {
                // 演示 LoadTableType 属性的用法
                LoadTableType = LoadNumbersTableType.OneTablePerSheet,
                
                // 其他最小必需属性
                Password = "password123",
                ParsingFormulaOnOpen = true
            };

            // 使用指定的加载选项加载 Numbers 文件
            Workbook workbook = new Workbook("sample.numbers", loadOptions);

            // 以 XLSX 格式保存工作簿
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* enum [LoadNumbersTableType](../../loadnumberstabletype/)
* class [NumbersLoadOptions](../)
* namespace [Aspose.Cells.Numbers](../../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../../)


