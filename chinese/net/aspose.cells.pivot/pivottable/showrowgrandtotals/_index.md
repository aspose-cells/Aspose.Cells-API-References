---
title: "PivotTable.ShowRowGrandTotals"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotTable 属性。指示是否在数据透视表的行中显示总计"
type: docs
url: /zh/net/aspose.cells.pivot/pivottable/showrowgrandtotals/
---
## PivotTable.ShowRowGrandTotals property

指示是否在数据透视表的行中显示总计。

```csharp
public bool ShowRowGrandTotals { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowRowGrandTotalsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 添加工作表
            Worksheet sheet = workbook.Worksheets[0];
            
            // 为数据透视表添加示例数据
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Product A";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "Product B";
            cells["B3"].Value = "South";
            cells["C3"].Value = 1500;
            
            cells["A4"].Value = "Product A";
            cells["B4"].Value = "South";
            cells["C4"].Value = 2000;
            
            cells["A5"].Value = "Product B";
            cells["B5"].Value = "North";
            cells["C5"].Value = 1200;

            // 添加数据透视表
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // 配置数据透视表
            pivotTable.ShowRowGrandTotals = true; // Demonstrate ShowRowGrandTotals property
            pivotTable.ShowColumnGrandTotals = true;
            
            // 将字段添加到区域
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product as row
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Region as column
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales as data
            
            // 保存工作簿
            workbook.Save("PivotTableShowRowGrandTotalsDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


