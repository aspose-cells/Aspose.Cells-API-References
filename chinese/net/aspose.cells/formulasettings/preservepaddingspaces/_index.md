---
title: "FormulaSettings.PreservePaddingSpaces"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "FormulaSettings 属性。指示在获取和设置公式时是否保留填充在公式标记之间的空格和换行符。默认值为 false"
type: docs
url: /zh/net/aspose.cells/formulasettings/preservepaddingspaces/
---
## FormulaSettings.PreservePaddingSpaces property

指示在获取和设置公式时是否保留填充在公式标记之间的空格和换行符。默认值为 false。

```csharp
public bool PreservePaddingSpaces { get; set; }
```

### 备注

通常这些空格和换行仅用于视觉目的，是否保留它们不会影响计算结果。出于性能考虑，如果没有特殊需求，处理公式时最好不要保留它们。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyPreservePaddingSpacesDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 设置带填充空格的公式
            string formulaWithSpaces = "=SUM( IF( A1:A5 > 10, B1:B5, 0 ) )";
            worksheet.Cells["C1"].Formula = formulaWithSpaces;
            
            // 默认行为（PreservePaddingSpaces 为 true）
            Console.WriteLine("Formula with spaces preserved: " + worksheet.Cells["C1"].Formula);
            
            // 更改设置以移除填充空格
            workbook.Settings.FormulaSettings.PreservePaddingSpaces = false;
            worksheet.Cells["C2"].Formula = formulaWithSpaces;
            
            Console.WriteLine("Formula with spaces removed: " + worksheet.Cells["C2"].Formula);
            
            // 保存工作簿
            workbook.Save("FormulaSpacesDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


