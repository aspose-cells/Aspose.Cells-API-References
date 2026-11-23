---
title: "Worksheet.CalculateArrayFormula"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Worksheet 方法。将公式计算为数组公式"
type: docs
url: /zh/net/aspose.cells/worksheet/calculatearrayformula/
---
## CalculateArrayFormula(string, CalculationOptions) {#calculatearrayformula}

将公式计算为数组公式。

```csharp
public object[][] CalculateArrayFormula(string formula, CalculationOptions opts)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 公式 | String | 待计算的公式。 |
| opts | CalculationOptions | 计算公式的选项 |

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateArrayFormulaWithStringCalculationOptionsDemo
    {
        public static void Run()
        {
            // 创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 填充一些示例数据
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(6);

            // 定义数组公式
            string arrayFormula = "=SUM(A1:B3)";
            
            // 使用计算选项计算数组公式
            object[][] result = worksheet.CalculateArrayFormula(arrayFormula, new CalculationOptions());
            
            // 输出结果
            Console.WriteLine("Result of array formula calculation: " + result[0][0]);
        }
    }
}
```

### 另请参见

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateArrayFormula(string, CalculationOptions, int, int) {#calculatearrayformula_1}

将公式计算为数组公式。

```csharp
public object[][] CalculateArrayFormula(string formula, CalculationOptions opts, int maxRowCount, 
    int maxColumnCount)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 公式 | String | 待计算的公式。 |
| opts | CalculationOptions | 计算公式的选项 |
| maxRowCount | Int32 | 结果数据的最大行数。如果为非正数或大于实际行数，则使用实际行数。 |
| maxColumnCount | Int32 | 结果数据的最大列数。如果它为非正数或大于实际行数，则使用实际列数。 |

### 返回值

已计算的公式结果。

### 备注

该公式将被视为动态数组公式，用于计算维度和结果。用户指定的最大维度用于计算结果为大数据集的情况（例如，计算结果可能对应整行或整列数据），但根据业务需求或性能考虑，用户并不需要如此大的数组。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateArrayFormulaWithStringCalculationOptionsInt32IDemo
    {
        public static void Run()
        {
            // 创建工作簿并访问第一个工作表
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // 示例 1：简单数组公式计算
            string formula = "=ISBLANK(IF(TRUE,B2:B5))";
            CalculationOptions options = new CalculationOptions();
            object[][] result = sheet.CalculateArrayFormula(formula, options, 1, 1);
            Console.WriteLine("Result of ISBLANK(IF(TRUE,B2:B5)): " + result[0][0]);

            // 示例 2：具有动态范围的数组公式
            formula = "=LEN(IF({1;2;3;4},B2:B5))";
            result = sheet.CalculateArrayFormula(formula, options, 1, 1);
            Console.WriteLine("Result of LEN(IF({1;2;3;4},B2:B5)): " + result[0][0]);

            // 示例 3：使用 MATCH 函数的数组公式
            // 设置一些测试数据
            sheet.Cells["B2"].PutValue(5);
            sheet.Cells["B3"].PutValue(10);
            sheet.Cells["C2"].PutValue(1);
            sheet.Cells["C3"].PutValue(2);
            sheet.Cells["D2"].PutValue(0);
            sheet.Cells["D3"].PutValue(0);

            formula = "=MATCH(1,IF(B2:B5=5,C2:C5,D2:D5),0)";
            result = sheet.CalculateArrayFormula(formula, options, 1, 1);
            Console.WriteLine("Result of MATCH formula: " + result[0][0]);
        }
    }
}
```

### 另请参见

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateArrayFormula(string, FormulaParseOptions, CalculationOptions, int, int, int, int, CalculationData) {#calculatearrayformula_2}

将公式计算为数组公式。

```csharp
public object[][] CalculateArrayFormula(string formula, FormulaParseOptions pOpts, 
    CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, 
    int maxColumnCount, CalculationData calculationData)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 公式 | String | 待计算的公式。 |
| pOpts | FormulaParseOptions | 解析公式的选项 |
| cOpts | CalculationOptions | 计算公式的选项 |
| baseCellRow | Int32 | 基准单元格的行索引。 |
| baseCellColumn | Int32 | 基准单元格的列索引。 |
| maxRowCount | Int32 | 结果数据的最大行数。如果它为非正数或大于实际行数，则使用实际行数。 |
| maxColumnCount | Int32 | 结果数据的最大列数。如果它为非正数或大于实际行数，则使用实际列数。 |
| calculationData | CalculationData | 计算数据。它用于用户在实现自定义计算引擎时需要计算一些静态公式的情况。对于此类情况，用户需要使用为 [`Calculate`](../../abstractcalculationengine/calculate/) 提供的计算数据来指定它。 |

### 返回值

已计算的公式结果。

### 备注

该公式将被视为动态数组公式，用于计算维度和结果。用户指定的最大维度用于计算结果为大数据集的情况（例如，计算结果可能对应整行或整列数据），但根据业务需求或性能考虑，用户并不需要如此大的数组。

### 另请参见

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [CalculationData](../../calculationdata/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


