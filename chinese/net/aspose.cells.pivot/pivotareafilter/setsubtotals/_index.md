---
title: "PivotAreaFilter.SetSubtotals"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotAreaFilter method. 过滤器的小计"
type: docs
url: /zh/net/aspose.cells.pivot/pivotareafilter/setsubtotals/
---
## PivotAreaFilter.SetSubtotals method

过滤器的汇总。

```csharp
public void SetSubtotals(PivotFieldSubtotalType subtotalType, bool shown)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | 小计函数。 |
| shown | 布尔 | 指示是否显示此小计数据。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaFilterMethodSetSubtotalsWithPivotFieldSubtotalTypeBooleanDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为数据透视表创建示例数据
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 8;

            // 创建数据透视表
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("=A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // 使用透视表参数创建透视区域
            PivotArea pivotArea = new PivotArea(pivotTable);
            PivotAreaFilter filter = new PivotAreaFilter();

            try
            {
                // 调用 SetSubtotals，使用 Sum 小计类型并设置为显示
                filter.SetSubtotals(PivotFieldSubtotalType.Sum, true);
                
                // 验证是否已设置小计
                bool isSumSet = filter.IsSubtotalSet(PivotFieldSubtotalType.Sum);
                Console.WriteLine($"Sum subtotal is set: {isSumSet}");

                // 刷新透视表以查看更改
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetSubtotals method: {ex.Message}");
            }
            
            // 保存结果
            workbook.Save("PivotAreaFilterSetSubtotalsDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotAreaFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


