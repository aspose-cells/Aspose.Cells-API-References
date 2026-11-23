---
title: "Range.UnionRanges"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Range 方法。返回两个范围的并集结果"
type: docs
url: /zh/net/aspose.cells/range/unionranges/
---
## Range.UnionRanges method

返回两个范围的并集结果。

```csharp
public UnionRange UnionRanges(Range[] ranges)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 范围 | Range[] | 该范围 |

### 返回值

两个范围的并集。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodUnionRangesWithRangeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 在单元格中创建示例数据
            worksheet.Cells["A1"].PutValue("Range 1");
            worksheet.Cells["B1"].PutValue("Data 1");
            worksheet.Cells["C1"].PutValue("Data 2");
            worksheet.Cells["A5"].PutValue("Range 2");
            worksheet.Cells["B5"].PutValue("Data 3");
            worksheet.Cells["C5"].PutValue("Data 4");

            // 创建要合并的范围
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:C3");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A5:C7");

            try
            {
                // 使用 Range[] 参数调用 UnionRanges
                Aspose.Cells.Range[] rangesToUnion = new Aspose.Cells.Range[] { range1, range2 };
                UnionRange unionRange = range1.UnionRanges(rangesToUnion);

                // 应用样式以显示联合范围
                Style style = workbook.CreateStyle();
                style.BackgroundColor = System.Drawing.Color.LightBlue;
                unionRange.ApplyStyle(style, new StyleFlag { All = true });

                Console.WriteLine($"Union range created successfully. Address: {unionRange.RefersTo}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnionRanges method: {ex.Message}");
            }

            // 保存结果
            workbook.Save("UnionRangesDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [UnionRange](../../unionrange/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


