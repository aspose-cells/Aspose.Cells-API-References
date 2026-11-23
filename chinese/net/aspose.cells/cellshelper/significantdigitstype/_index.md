---
title: "CellsHelper.SignificantDigitsType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "CellsHelper 属性。获取和设置用于输出数值的默认有效数字类型。默认值为 G17"
type: docs
url: /zh/net/aspose.cells/cellshelper/significantdigitstype/
---
## CellsHelper.SignificantDigitsType property

获取和设置用于输出数值的默认有效数字类型。默认值为 G17。

```csharp
public static SignificantDigitsType SignificantDigitsType { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperPropertySignificantDigitsTypeDemo
    {
        public static void Run()
        {
            try
            {
                // 显示当前 SignificantDigitsType 值
                Console.WriteLine("Current SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // 设置新的 SignificantDigitsType 值
                CellsHelper.SignificantDigitsType = SignificantDigitsType.G17;
                Console.WriteLine("Updated SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // 创建工作簿以演示效果
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // 添加一个将受有效数字影响的数值
                worksheet.Cells["A1"].PutValue(1.2345678912345678);
                worksheet.Cells["A2"].PutValue(1.2345678912345678);
                worksheet.Cells["A3"].Formula = "=A1+A2";

                // 使用当前的有效数字类型计算公式
                workbook.CalculateFormula();

                // 显示结果
                Console.WriteLine("Calculation result: " + worksheet.Cells["A3"].Value);

                // 更改为另一种有效数字类型
                CellsHelper.SignificantDigitsType = SignificantDigitsType.Rounding17;
                Console.WriteLine("Changed SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // 使用新的有效数字类型重新计算
                workbook.CalculateFormula();
                Console.WriteLine("Recalculated result: " + worksheet.Cells["A3"].Value);

                // 保存工作簿
                workbook.Save("SignificantDigitsTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* enum [SignificantDigitsType](../../significantdigitstype/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


