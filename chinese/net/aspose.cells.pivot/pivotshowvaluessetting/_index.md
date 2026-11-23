---
title: "类 PivotShowValuesSetting"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Pivot.PivotShowValuesSetting 类。表示在使用 ShowDataAs 计算时关于显示值的设置"
type: docs
url: /zh/net/aspose.cells.pivot/pivotshowvaluessetting/
---
## PivotShowValuesSetting class

表示在使用 ShowDataAs 计算时关于显示值的设置。

```csharp
public class PivotShowValuesSetting
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [BaseFieldIndex](../../aspose.cells.pivot/pivotshowvaluessetting/basefieldindex/) { get; set; } | 表示在使用 ShowDataAs 计算时的 ShowDataAs 计算的基字段。 |
| [BaseFieldName](../../aspose.cells.pivot/pivotshowvaluessetting/basefieldname/) { get; } | 获取透视基字段的标题。 |
| [BaseItemCaption](../../aspose.cells.pivot/pivotshowvaluessetting/baseitemcaption/) { get; } | 获取基字段中透视项的标题。 |
| [BaseItemIndex](../../aspose.cells.pivot/pivotshowvaluessetting/baseitemindex/) { get; set; } | 表示在使用 ShowDataAs 计算时基字段中透视项的自定义索引。 |
| [BaseItemPositionType](../../aspose.cells.pivot/pivotshowvaluessetting/baseitempositiontype/) { get; set; } | (**Obsolete.**) 表示在使用 ShowDataAs 计算时，基字段中基础数据透视项的类型。由于 PivotItemPosition.Custom 仅用于读取，如果需要设置 PivotItemPosition.Custom，请设置 PivotField.BaseItemIndex 属性。 |
| [CalculationType](../../aspose.cells.pivot/pivotshowvaluessetting/calculationtype/) { get; set; } | (**Obsolete.**) 表示在数据透视报告中如何显示数据字段的值。 |
| [ShowValuesAs](../../aspose.cells.pivot/pivotshowvaluessetting/showvaluesas/) { get; set; } | 获取和设置在数据透视报告中如何显示数据字段的值。 |

## 字段

| 名称 | 描述 |
| --- | --- |
| const [NextPivotItem](../../aspose.cells.pivot/pivotshowvaluessetting/nextpivotitem/) | 特殊基项索引：使用后续的数据透视项。适用于 "Show Values As" 计算；在 Excel 2010 及更高版本中有效。 |
| const [PreviousPivotItem](../../aspose.cells.pivot/pivotshowvaluessetting/previouspivotitem/) | 特殊基项索引：使用前面的数据透视项。适用于 "Show Values As" 计算；在 Excel 2010 及更高版本中有效。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotShowValuesSettingDemo
    {
        public static void PivotShowValuesSettingExample()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 向工作表添加一些数据
            worksheet.Cells[0, 0].Value = "Product";
            worksheet.Cells[0, 1].Value = "Sales";
            worksheet.Cells[1, 0].Value = "A";
            worksheet.Cells[1, 1].Value = 100;
            worksheet.Cells[2, 0].Value = "B";
            worksheet.Cells[2, 1].Value = 150;
            worksheet.Cells[3, 0].Value = "C";
            worksheet.Cells[3, 1].Value = 200;

            // 向工作表添加透视表
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // 向数据透视表添加字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

            // 访问数据字段
            PivotField dataField = pivotTable.DataFields[0];

            // 访问 ShowValuesSetting 属性
            PivotShowValuesSetting showValuesSetting = dataField.ShowValuesSetting;

            // 设置 PivotShowValuesSetting 的属性
            showValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;
            showValuesSetting.BaseFieldIndex = 0; // Base field index
            showValuesSetting.BaseItemPositionType = PivotItemPositionType.Next;
            showValuesSetting.BaseItemIndex = 1; // Base item index

            // 刷新并计算数据透视表数据
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // 保存工作簿
            workbook.Save("PivotShowValuesSettingExample.xlsx");

            return;
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


