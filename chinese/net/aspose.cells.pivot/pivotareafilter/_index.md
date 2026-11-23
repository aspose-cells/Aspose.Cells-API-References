---
title: "类 PivotAreaFilter"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Pivot.PivotAreaFilter 类。表示用于数据透视表的 PivotArea 过滤器"
type: docs
url: /zh/net/aspose.cells.pivot/pivotareafilter/
---
## PivotAreaFilter class

表示 [`PivotArea`](../pivotarea/) 对于 [`PivotTable`](../pivottable/) 的过滤器。

```csharp
public class PivotAreaFilter
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [PivotAreaFilter](pivotareafilter/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [FieldIndex](../../aspose.cells.pivot/pivotareafilter/fieldindex/) { get; } | 获取此过滤器所引用的源字段中字段的索引。值为 -2 表示值字段。 |
| [Selected](../../aspose.cells.pivot/pivotareafilter/selected/) { get; set; } | 指示此字段是否具有选择。仅在数据透视表处于大纲视图时有效。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [IsSubtotalSet](../../aspose.cells.pivot/pivotareafilter/issubtotalset/)(PivotFieldSubtotalType) | 获取为此过滤器设置的汇总方式。 |
| [SetSubtotals](../../aspose.cells.pivot/pivotareafilter/setsubtotals/)(PivotFieldSubtotalType, bool) | 过滤器的汇总。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotAreaFilterDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 示例数据设置
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["A3"].Value = "Car";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            
            // 创建数据透视表 - 修复返回值处理
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // 创建并配置 PivotAreaFilter
            PivotAreaFilter filter = new PivotAreaFilter();
            filter.Selected = true;
            filter.SetSubtotals(PivotFieldSubtotalType.Sum, true);
            
            // 演示方法
            bool isSumSet = filter.IsSubtotalSet(PivotFieldSubtotalType.Sum);
            Console.WriteLine($"Sum subtotal visibility set: {isSumSet}");
            
            workbook.Save("PivotAreaFilterDemo.xlsx");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


