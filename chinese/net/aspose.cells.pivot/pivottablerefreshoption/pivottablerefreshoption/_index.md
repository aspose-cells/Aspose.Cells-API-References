---
title: "PivotTableRefreshOption.PivotTableRefreshOption"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotTableRefreshOption 构造函数。 表示刷新枢轴表数据源的选项"
type: docs
url: /zh/net/aspose.cells.pivot/pivottablerefreshoption/pivottablerefreshoption/
---
## PivotTableRefreshOption constructor

表示刷新透视表数据源的选项。

```csharp
public PivotTableRefreshOption()
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableRefreshOptionMethodCtorDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 为数据透视表添加示例数据
            var cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Apple";
            cells["B2"].Value = "North";            cells["C2"].Value = 1000;
            cells["A3"].Value = "Orange";            cells["B3"].Value = "South";            cells["C3"].Value = 2000;
            cells["A4"].Value = "Banana";            cells["B4"].Value = "East";            cells["C4"].Value = 3000;
            cells["A5"].Value = "Apple";            cells["B5"].Value = "South";            cells["C5"].Value = 4000;
            
            // 创建数据透视表
            int index = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // 向数据透视表添加字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // 使用构造函数创建并配置刷新选项
            PivotTableRefreshOption refreshOption = new PivotTableRefreshOption();
            refreshOption.ReserveMissingPivotItemType = ReserveMissingPivotItemType.None;
            
            // 使用选项刷新枢轴表
            pivotTable.RefreshData(refreshOption);
            pivotTable.CalculateData();
            
            // 保存工作簿
            workbook.Save("PivotTableRefreshDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### 另请参见

* class [PivotTableRefreshOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


