---
title: "ReferredArea.IsEntireColumn"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ReferredArea 属性。指示此区域是否包含所有行（整个列）"
type: docs
url: /zh/net/aspose.cells/referredarea/isentirecolumn/
---
## ReferredArea.IsEntireColumn property

指示此区域是否包含所有行（整个列）。

```csharp
public bool IsEntireColumn { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ReferredAreaPropertyIsEntireColumnDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加示例数据
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);

            // 创建一个引用整列 B 的命名范围
            int index = workbook.Worksheets.Names.Add("PriceColumn");
            workbook.Worksheets.Names[index].RefersTo = "=Sheet1!$B:$B";

            // 获取该命名范围的引用区域
            ReferredArea referredArea = workbook.Worksheets.Names["PriceColumn"].GetReferredAreas(false)[0];

            // 显示 IsEntireColumn 属性值
            Console.WriteLine("IsEntireColumn value for PriceColumn: " + referredArea.IsEntireColumn);

            // 创建另一个引用特定范围（非整列）的命名范围
            int index2 = workbook.Worksheets.Names.Add("ProductRange");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$A$1:$B$3";

            // 获取第二个命名范围的引用区域
            ReferredArea referredArea2 = workbook.Worksheets.Names["ProductRange"].GetReferredAreas(false)[0];

            // 显示第二个范围的 IsEntireColumn 属性值
            Console.WriteLine("IsEntireColumn value for ProductRange: " + referredArea2.IsEntireColumn);

            // 通过检查范围维度演示 IsEntireColumn 的效果
            Console.WriteLine("PriceColumn dimensions: StartRow={0}, EndRow={1}, StartColumn={2}, EndColumn={3}",
                referredArea.StartRow, referredArea.EndRow, referredArea.StartColumn, referredArea.EndColumn);

            Console.WriteLine("ProductRange dimensions: StartRow={0}, EndRow={1}, StartColumn={2}, EndColumn={3}",
                referredArea2.StartRow, referredArea2.EndRow, referredArea2.StartColumn, referredArea2.EndColumn);

            // 保存工作簿
            workbook.Save("ReferredAreaPropertyIsEntireColumnDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


