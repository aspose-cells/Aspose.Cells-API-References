---
title: "AdvancedFilter.CopyToRange"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "AdvancedFilter 属性。获取将此高级筛选器的结果复制到的范围"
type: docs
url: /zh/net/aspose.cells/advancedfilter/copytorange/
---
## AdvancedFilter.CopyToRange property

获取将此高级筛选结果复制到的范围。

```csharp
public string CopyToRange { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AdvancedFilterPropertyCopyToRangeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 获取第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];

            // 向工作表添加示例数据
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1.5);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(0.8);
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(1.2);

            // 添加条件范围
            worksheet.Cells["D1"].PutValue("Product");
            worksheet.Cells["D2"].PutValue("Apple");

            try
            {
                // 从工作表获取 AdvancedFilter 实例
                AdvancedFilter advancedFilter = worksheet.GetAdvancedFilter();

                // 显示 CopyToRange 属性值
                Console.WriteLine("CopyToRange value: " + advancedFilter.CopyToRange);

                // 保存工作簿
                workbook.Save("CopyToRangeDemo.xlsx");
                Console.WriteLine("CopyToRange demonstration completed successfully.");
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

* class [AdvancedFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


