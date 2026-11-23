---
title: "类 PivotTableRefreshOption"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Pivot.PivotTableRefreshOption 类。表示刷新透视表数据源的选项"
type: docs
url: /zh/net/aspose.cells.pivot/pivottablerefreshoption/
---
## PivotTableRefreshOption class

表示刷新透视表数据源的选项。

```csharp
public class PivotTableRefreshOption
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [PivotTableRefreshOption](pivottablerefreshoption/)() | 表示刷新透视表数据源的选项。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [IsKeepOriginalOrder](../../aspose.cells.pivot/pivottablerefreshoption/iskeeporiginalorder/) { get; set; } | 指示是否保持透视项的原始顺序与旧数据源相同。 |
| [KeepCachedLocalGroupData](../../aspose.cells.pivot/pivottablerefreshoption/keepcachedlocalgroupdata/) { get; set; } | 指示在最大值和最小值保持不变时是否保留缓存的本地分组数据。默认值为 false，表示使用本地设置刷新分组。 |
| [ReserveMissingPivotItemType](../../aspose.cells.pivot/pivottablerefreshoption/reservemissingpivotitemtype/) { get; set; } | 表示如何保留缺失的透视项。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableRefreshOptionDemo
    {
        public static void PivotTableRefreshOptionExample()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 向工作表添加一些数据
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 0].Value = "Apple";
            worksheet.Cells[3, 1].Value = 2021;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 0].Value = "Banana";
            worksheet.Cells[4, 1].Value = 2021;
            worksheet.Cells[4, 2].Value = 80;

            // 向工作表添加透视表
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // 向数据透视表添加字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // 创建 PivotTableRefreshOption 的实例
            PivotTableRefreshOption refreshOption = new PivotTableRefreshOption
            {
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // 使用指定的选项刷新透视表
            pivotTable.RefreshData(refreshOption);
            pivotTable.CalculateData();

            // 保存工作簿
            workbook.Save("PivotTableRefreshOptionExample.xlsx");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


