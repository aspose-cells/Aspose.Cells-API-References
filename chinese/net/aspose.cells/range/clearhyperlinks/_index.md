---
title: "Range.ClearHyperlinks"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Range 方法。仅删除超链接"
type: docs
url: /zh/net/aspose.cells/range/clearhyperlinks/
---
## Range.ClearHyperlinks method

仅删除超链接。

```csharp
public void ClearHyperlinks(bool clearFormat)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| clearFormat | 布尔 | 指示是否清除超链接的格式。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearHyperlinksWithBooleanDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建一个范围并添加一些超链接用于演示
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");
            range.AddHyperlink("https://www.aspose.com", "Aspose", "Visit Aspose");
            range.AddHyperlink("https://www.example.com", "Example", "Visit Example");

            try
            {
                // 在保留格式的情况下清除超链接（false）
                range.ClearHyperlinks(false);
                Console.WriteLine("Hyperlinks cleared while preserving format");

                // 再次添加超链接
                range.AddHyperlink("https://www.aspose.com", "Aspose", "Visit Aspose");

                // 在不保留格式的情况下清除超链接（true）
                range.ClearHyperlinks(true);
                Console.WriteLine("Hyperlinks cleared without preserving format");

                // 保存工作簿
                workbook.Save("ClearHyperlinksDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
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


