---
title: "PivotShowValuesSetting.BaseItemIndex"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotShowValuesSetting 属性。表示在使用 ShowDataAs 计算时基字段中透视项的自定义索引"
type: docs
url: /zh/net/aspose.cells.pivot/pivotshowvaluessetting/baseitemindex/
---
## PivotShowValuesSetting.BaseItemIndex property

表示在使用 ShowDataAs 计算时基字段中透视项的自定义索引。

```csharp
public int BaseItemIndex { get; set; }
```

### 备注

[`PreviousPivotItem`](../previouspivotitem/) (-1) for the preceding item, [`NextPivotItem`](../nextpivotitem/) (-2) for the succeeding item; non‑negative values denote the ordinal index of a specific pivot item.

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotShowValuesSettingPropertyBaseItemIndexDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 示例数据
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["A4"].Value = "C";
            worksheet.Cells["B4"].Value = 200;

            // 创建数据透视表
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // 配置显示值设置
            PivotField dataField = pivotTable.DataFields[0];
            dataField.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOf;
            dataField.ShowValuesSetting.BaseFieldIndex = 0;
            dataField.ShowValuesSetting.BaseItemIndex = 1; // Using BaseItemIndex property

            pivotTable.RefreshData();
            pivotTable.CalculateData();

            workbook.Save("PivotShowValuesSettingBaseItemIndexDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotShowValuesSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


