---
title: "PivotField.ShowValuesSetting"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotField 属性。获取在使用 ShowDataAs 计算时显示值的设置"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfield/showvaluessetting/
---
## PivotField.ShowValuesSetting property

获取在使用 ShowDataAs 计算时显示值的设置。

```csharp
public PivotShowValuesSetting ShowValuesSetting { get; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyShowValuesSettingDemo
    {
        public static void Run()
        {
            // 创建工作簿
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // 为数据透视表添加示例数据
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 3000;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 1500;
            cells["A6"].Value = "Orange";
            cells["B6"].Value = 2500;
            cells["A7"].Value = "Banana";
            cells["B7"].Value = 3500;

            // 创建数据透视表
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B7", "C10", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // 添加行字段和数据字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[0];
            
            // 配置 ShowValuesSetting 以显示为总计的百分比
            dataField.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;
            
            // 计算并刷新透视表
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // 保存工作簿
            workbook.Save("PivotFieldShowValuesSettingDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotShowValuesSetting](../../pivotshowvaluessetting/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


