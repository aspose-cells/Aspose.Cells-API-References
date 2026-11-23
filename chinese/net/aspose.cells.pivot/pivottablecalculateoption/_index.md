---
title: "类 PivotTableCalculateOption"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Pivot.PivotTableCalculateOption 类。表示数据透视表数据计算的选项"
type: docs
url: /zh/net/aspose.cells.pivot/pivottablecalculateoption/
---
## PivotTableCalculateOption class

表示数据透视表数据计算的选项。

```csharp
public class PivotTableCalculateOption
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [PivotTableCalculateOption](pivottablecalculateoption/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [RefreshCharts](../../aspose.cells.pivot/pivottablecalculateoption/refreshcharts/) { get; set; } | 指示是否基于此数据透视表刷新图表。 |
| [RefreshData](../../aspose.cells.pivot/pivottablecalculateoption/refreshdata/) { get; set; } | 指示是否刷新数据透视表的数据源。 |
| [RefreshOption](../../aspose.cells.pivot/pivottablecalculateoption/refreshoption/) { get; set; } | 获取和设置刷新数据源到数据透视缓存的选项。 |
| [ReserveMissingPivotItemType](../../aspose.cells.pivot/pivottablecalculateoption/reservemissingpivotitemtype/) { get; set; } | 表示如何保留缺失的透视项。 |

### 示例

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotTableCalculateOptionDemo
    {
        public static void PivotTableCalculateOptionExample()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // 为数据透视表添加一些数据
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["B3"].PutValue(30);
            sheet.Cells["A4"].PutValue("Fruit");
            sheet.Cells["B4"].PutValue(70);
            sheet.Cells["A5"].PutValue("Vegetable");
            sheet.Cells["B5"].PutValue(40);

            // 向工作表添加透视表
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // 配置数据透视表
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount

            // 创建 PivotTableCalculateOption 对象
            PivotTableCalculateOption calculateOption = new PivotTableCalculateOption
            {
                RefreshData = true,
                RefreshCharts = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // 使用指定的选项计算数据透视表数据
            pivotTable.CalculateData(calculateOption);

            // 保存工作簿
            workbook.Save("PivotTableCalculateOptionExample.xlsx");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


