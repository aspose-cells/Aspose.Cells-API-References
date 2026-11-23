---
title: "ListColumn.TotalsRowLabel"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ListColumn 属性。获取和设置合计行的显示标签"
type: docs
url: /zh/net/aspose.cells.tables/listcolumn/totalsrowlabel/
---
## ListColumn.TotalsRowLabel property

获取和设置合计行的显示标签。

```csharp
public string TotalsRowLabel { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyTotalsRowLabelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 添加示例数据
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["A4"].PutValue("Item3");
            worksheet.Cells["B4"].PutValue(200);

            // 创建表格
            int index = worksheet.ListObjects.Add(0, 0, 4, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.ShowTotals = true;

            // 配置合计行
            ListColumn priceColumn = table.ListColumns[1];
            priceColumn.TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;
            priceColumn.TotalsRowLabel = "Grand Total";

            workbook.Save("ListColumnTotalsRowLabelDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


