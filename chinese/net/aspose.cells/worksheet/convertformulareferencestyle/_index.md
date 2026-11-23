---
title: "Worksheet.ConvertFormulaReferenceStyle"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Worksheet method. 转换公式引用样式"
type: docs
url: /zh/net/aspose.cells/worksheet/convertformulareferencestyle/
---
## Worksheet.ConvertFormulaReferenceStyle method

转换公式引用样式。

```csharp
public string ConvertFormulaReferenceStyle(string formula, bool toR1C1, int baseCellRow, 
    int baseCellColumn)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 公式 | String | 待转换的公式。 |
| toR1C1 | 布尔 | 要将公式转换为何种引用样式。若原公式使用 A1 引用样式，则此值应为 true，以便公式从 A1 转换为 R1C1 引用样式；若原公式使用 R1C1 引用样式，则此值应为 false，以便公式从 R1C1 转换为 A1 引用样式； |
| baseCellRow | Int32 | 基准单元格的行索引。 |
| baseCellColumn | Int32 | 基准单元格的列索引。 |

### 返回值

已转换的公式。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodConvertFormulaReferenceStyleWithStringBooleanInt32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // 示例 1：将 R1C1 样式转换为 A1 样式
            string formulaR1C1 = "R[0]C23,testDS,R[0]C24";
            string formulaA1 = sheet.ConvertFormulaReferenceStyle(formulaR1C1, false, 0, 0);
            Console.WriteLine("Converted formula: " + formulaA1);

            // 示例 2：使用混合引用进行转换
            string formulaMixed = "R[0]C23,testDS,rcurr,R[0]C24";
            string convertedMixed = sheet.ConvertFormulaReferenceStyle(formulaMixed, false, 0, 0);
            Console.WriteLine("Converted mixed formula: " + convertedMixed);
        }
    }
}
```

### 另请参见

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


