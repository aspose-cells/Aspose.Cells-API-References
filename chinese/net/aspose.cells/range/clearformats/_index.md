---
title: "Range.ClearFormats"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Range 方法。清除此范围的格式"
type: docs
url: /zh/net/aspose.cells/range/clearformats/
---
## Range.ClearFormats method

清除此范围的格式。

```csharp
public void ClearFormats()
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearFormatsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一些带格式的数据
            Cell cell = worksheet.Cells["A1"];
            cell.Value = "Formatted Cell";
            cell.GetStyle().Font.IsBold = true;
            cell.GetStyle().ForegroundColor = System.Drawing.Color.Yellow;
            cell.GetStyle().Pattern = BackgroundType.Solid;

            // 创建一个范围
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B5");

            try
            {
                // 清除范围的格式
                range.ClearFormats();

                Console.WriteLine("Formats cleared successfully from range A1:B5");
                Console.WriteLine($"Cell A1 value after clearing formats: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"Cell A1 is bold after clearing formats: {worksheet.Cells["A1"].GetStyle().Font.IsBold}");

                // 保存工作簿
                workbook.Save("ClearFormatsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ClearFormats: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


