---
title: "Range.UnionRang"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Range 方法。返回两个范围的并集结果"
type: docs
url: /zh/net/aspose.cells/range/unionrang/
---
## Range.UnionRang method

返回两个范围的并集结果。

```csharp
[Obsolete("Use Range.UnionRanges() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Range[] UnionRang(Range range)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 范围 | 范围 | 该范围 |

### 返回值

两个范围的并集。

### 备注

注意：此方法现已过时。请改用 Range.UnionRanges() 方法。该方法将在自 2024 年 5 月起的 12 个月后被移除。Aspose 对您可能遇到的任何不便表示歉意。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using Range = Aspose.Cells.Range; // Add this alias to resolve ambiguity

    public class RangeMethodUnionRangWithRangeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建两个范围以演示 UnionRang
            Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Range range2 = worksheet.Cells.CreateRange("C3:D4");

            // 为可视化在范围中设置一些值
            range1[0, 0].PutValue("Range1");
            range1[1, 1].PutValue("Data");
            range2[0, 0].PutValue("Range2");
            range2[1, 1].PutValue("Data");

            try
            {
                // 调用 UnionRang 方法以合并这两个范围
                Range[] unionResult = range1.UnionRang(range2);

                // 显示有关联合结果的信息
                Console.WriteLine("UnionRang method executed successfully.");
                Console.WriteLine($"Number of ranges in union: {unionResult.Length}");
                Console.WriteLine($"First union range address: {unionResult[0].Address}");
                Console.WriteLine($"Second union range address: {unionResult[1].Address}");

                // 为可视化在联合范围上添加边框标记
                foreach (Range r in unionResult)
                {
                    r.SetOutlineBorders(CellBorderType.Thin, System.Drawing.Color.Black);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnionRang method: {ex.Message}");
            }

            // 保存结果
            workbook.Save("RangeMethodUnionRangWithRangeDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


