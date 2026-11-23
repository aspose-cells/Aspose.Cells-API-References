---
title: "Range.ClearContents"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Range 方法。清除此范围的内容"
type: docs
url: /zh/net/aspose.cells/range/clearcontents/
---
## Range.ClearContents method

清除此范围的内容。

```csharp
public void ClearContents()
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearContentsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一些示例数据以演示清除
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            worksheet.Cells["A2"].PutValue("Sample");
            worksheet.Cells["B2"].PutValue("Data");

            try
            {
                // 创建一个覆盖单元格 A1:B2 的范围
                Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");

                // 显示清除前的范围内容
                Console.WriteLine("Before clearing:");
                Console.WriteLine($"A1: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"B1: {worksheet.Cells["B1"].Value}");
                Console.WriteLine($"A2: {worksheet.Cells["A2"].Value}");
                Console.WriteLine($"B2: {worksheet.Cells["B2"].Value}");

                // 调用 ClearContents 来移除范围内的所有值
                range.ClearContents();

                // 显示清除后的范围内容
                Console.WriteLine("\nAfter clearing:");
                Console.WriteLine($"A1: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"B1: {worksheet.Cells["B1"].Value}");
                Console.WriteLine($"A2: {worksheet.Cells["A2"].Value}");
                Console.WriteLine($"B2: {worksheet.Cells["B2"].Value}");

                // 保存工作簿
                workbook.Save("ClearContentsDemo.xlsx");
                Console.WriteLine("\nWorkbook saved successfully.");
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

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


