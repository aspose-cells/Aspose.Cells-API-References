---
title: "PivotShowValuesSetting.BaseItemPositionType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotShowValuesSetting 属性。表示在使用 ShowDataAs 计算时基字段中基透视项的类型。由于 PivotItemPosition.Custom 仅用于只读，如果需要设置 PivotItemPosition.Custom，请设置 PivotField.BaseItemIndex 属性"
type: docs
url: /zh/net/aspose.cells.pivot/pivotshowvaluessetting/baseitempositiontype/
---
## PivotShowValuesSetting.BaseItemPositionType property

表示在使用 ShowDataAs 计算时基字段中基透视项的类型。由于 PivotItemPosition.Custom 仅用于只读，如果需要设置 PivotItemPosition.Custom，请设置 PivotField.BaseItemIndex 属性。

```csharp
[Obsolete("Use PivotShowValuesSetting.BaseItem property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotItemPositionType BaseItemPositionType { get; set; }
```

### 备注

注意：此属性现已过时。请改用 PivotShowValuesSetting.BaseItem 属性。此方法将在自 2026 年 11 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotShowValuesSettingPropertyBaseItemPositionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells[0, 0].Value = "Product";
            worksheet.Cells[0, 1].Value = "Sales";
            worksheet.Cells[1, 0].Value = "A";
            worksheet.Cells[1, 1].Value = 100;
            worksheet.Cells[2, 0].Value = "B";
            worksheet.Cells[2, 1].Value = 150;
            worksheet.Cells[3, 0].Value = "C";
            worksheet.Cells[3, 1].Value = 200;

            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            PivotField dataField = pivotTable.DataFields[0];
            PivotShowValuesSetting showValuesSetting = dataField.ShowValuesSetting;

            showValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;
            showValuesSetting.BaseFieldIndex = 0;
            showValuesSetting.BaseItemPositionType = PivotItemPositionType.Next;
            showValuesSetting.BaseItemIndex = 1;

            pivotTable.RefreshData();
            pivotTable.CalculateData();

            workbook.Save("PivotShowValuesSettingExample.xlsx");
        }
    }
}
```

### 另请参见

* enum [PivotItemPositionType](../../pivotitempositiontype/)
* class [PivotShowValuesSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


