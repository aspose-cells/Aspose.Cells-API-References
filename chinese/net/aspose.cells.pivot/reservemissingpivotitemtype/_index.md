---
title: "枚举 ReserveMissingPivotItemType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Pivot.ReserveMissingPivotItemType 枚举。表示如何保留缺失的数据透视项。"
type: docs
url: /zh/net/aspose.cells.pivot/reservemissingpivotitemtype/
---
## ReserveMissingPivotItemType enumeration

表示如何保留缺失的数据透视项。

```csharp
public enum ReserveMissingPivotItemType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Default | `0` | 删除旧的缺失数据透视项，并将新数据源中删除的项保留为缺失项。 |
| All | `1` | 保留所有缺失项。 |
| None | `2` | 删除所有缺失的数据透视项。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class ReserveMissingPivotItemTypeDemo
    {
        public static void ReserveMissingPivotItemTypeExample()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 向工作簿添加新工作表
            Worksheet worksheet = workbook.Worksheets[0];

            // 向工作表添加示例数据
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // 向工作表添加数据透视表
            int pivotTableIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // 向数据透视表添加字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // 设置 ReserveMissingPivotItemType 选项
            PivotTableCalculateOption calculateOption = new PivotTableCalculateOption
            {
                RefreshData = true,
                RefreshCharts = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // 使用指定的选项计算透视表
            pivotTable.CalculateData(calculateOption);

            // 刷新透视表
            pivotTable.RefreshData();

            // 保存工作簿
            workbook.Save("ReserveMissingPivotItemTypeExample.xlsx");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


