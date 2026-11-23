---
title: "PivotTableCalculateOption.ReserveMissingPivotItemType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotTableCalculateOption 属性。表示如何保留缺失的透视项"
type: docs
url: /zh/net/aspose.cells.pivot/pivottablecalculateoption/reservemissingpivotitemtype/
---
## PivotTableCalculateOption.ReserveMissingPivotItemType property

表示如何保留缺失的透视项。

```csharp
public ReserveMissingPivotItemType ReserveMissingPivotItemType { get; set; }
```

### 备注

仅在 [`RefreshData`](../refreshdata/) 为 true 时有效。

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCalculateOptionPropertyReserveMissingPivotItemTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // 示例数据
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["A4"].PutValue("A");
            sheet.Cells["B4"].PutValue(30);

            // 创建数据透视表
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // 配置透视字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // 使用 ReserveMissingPivotItemType 设置计算选项
            PivotTableCalculateOption options = new PivotTableCalculateOption
            {
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // 使用选项进行计算
            pivotTable.CalculateData(options);

            // 保存结果
            workbook.Save("PivotTableReserveMissingItemsDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [ReserveMissingPivotItemType](../../reservemissingpivotitemtype/)
* class [PivotTableCalculateOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


