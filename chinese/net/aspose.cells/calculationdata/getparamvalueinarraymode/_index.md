---
title: "CalculationData.GetParamValueInArrayMode"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "CalculationData 方法。获取给定索引处参数的值。如果参数是需要计算的某种表达式，则将在数组模式下进行计算"
type: docs
url: /zh/net/aspose.cells/calculationdata/getparamvalueinarraymode/
---
## CalculationData.GetParamValueInArrayMode method

获取给定索引处参数的值。如果参数是需要计算的某种表达式，则将在数组模式下进行计算。

```csharp
public object[][] GetParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | Int32 | 参数的索引（从 0 开始） |
| maxRowCount | Int32 | 返回数组的行数限制。如果该值为非正数或大于实际行数，则使用实际行数。 |
| maxColumnCount | Int32 | 返回数组的列数限制。如果该值为非正数或大于实际行数，则使用实际列数。 |

### 返回值

一个数组，包含指定参数表示的所有项。

### 备注

对于需要计算的表达式，以 A:A+B:B 为例：在值模式下，它会根据当前单元格基准计算为单个值。但在数组模式下，A1+B1、A2+B2、A3+B3、... 的所有值都会被计算并用于构建返回的数组。对于这种情况，最好指定行/列计数的上限（例如根据 [`MaxDataRow`](../../cells/maxdatarow/) 和 [`MaxDataColumn`](../../cells/maxdatacolumn/)），否则返回的大数组可能会因大量无用数据而增加内存开销。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataMethodGetParamValueInArrayModeWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加示例数据以供上下文使用
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Formula = "=SUM(A1:C3)";

            try
            {
                // 使用自定义引擎创建计算选项
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new ArrayModeCalculationEngine();
                workbook.CalculateFormula(options);

                Console.WriteLine("GetParamValueInArrayMode method called successfully");
                workbook.Save("GetParamValueInArrayModeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetParamValueInArrayMode: {ex.Message}");
            }
        }

        private class ArrayModeCalculationEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                if (data.FunctionName == "SUM")
                {
                    // 使用真实参数调用 GetParamValueInArrayMode
                    object[][] paramArray = data.GetParamValueInArrayMode(0, 5, 3);

                    Console.WriteLine($"Parameter array dimensions: {paramArray.Length} rows");
                    if (paramArray.Length > 0)
                    {
                        Console.WriteLine($"First row has {paramArray[0].Length} columns");
                    }
                }
            }
        }
    }
}
```

### 另请参见

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


