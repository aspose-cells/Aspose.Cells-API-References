---
title: "类 PivotArea"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Pivot.PivotArea 类。呈现透视表的选定区域"
type: docs
url: /zh/net/aspose.cells.pivot/pivotarea/
---
## PivotArea class

呈现透视表的选定区域。

```csharp
public class PivotArea
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [PivotArea](pivotarea/)(PivotTable) | 呈现 PivotTable 的选定区域。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [AxisType](../../aspose.cells.pivot/pivotarea/axistype/) { get; set; } | 获取并设置此规则适用的 PivotTable 区域。 |
| [Filters](../../aspose.cells.pivot/pivotarea/filters/) { get; } | 获取此 PivotArea 的所有筛选器。 |
| [IsColumnGrandIncluded](../../aspose.cells.pivot/pivotarea/iscolumngrandincluded/) { get; set; } | 指示是否包含列总计。 |
| [IsOutline](../../aspose.cells.pivot/pivotarea/isoutline/) { get; set; } | 指示规则是否引用处于大纲模式的区域。 |
| [IsRowGrandIncluded](../../aspose.cells.pivot/pivotarea/isrowgrandincluded/) { get; set; } | 指示是否包含行总计。 |
| [OnlyData](../../aspose.cells.pivot/pivotarea/onlydata/) { get; set; } | 指示是否仅选择项目选择的数据值（视图的数据区域），且不包括项目标签。 |
| [OnlyLabel](../../aspose.cells.pivot/pivotarea/onlylabel/) { get; set; } | 指示是否仅选择项目选择的数据标签。 |
| [RuleType](../../aspose.cells.pivot/pivotarea/ruletype/) { get; set; } | 获取并设置选择规则的类型。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [GetCellAreas](../../aspose.cells.pivot/pivotarea/getcellareas/)() | 获取此透视区域的单元格区域。 |
| [Select](../../aspose.cells.pivot/pivotarea/select/)(PivotFieldType, int, PivotTableSelectionType) | 使用筛选器选择区域。 |
| [SelectField](../../aspose.cells.pivot/pivotarea/selectfield/#selectfield)(PivotFieldType, PivotField) | 在区域中选择字段作为区域。 |
| [SelectField](../../aspose.cells.pivot/pivotarea/selectfield/#selectfield_1)(PivotFieldType, string) | 在区域中选择字段作为区域。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaDemo
    {
        public static void PivotAreaExample()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 向工作表添加一些数据
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[3, 0].Value = "Cherry";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2021;
            worksheet.Cells[3, 1].Value = 2022;
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;

            // 向工作表添加透视表
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // 向数据透视表添加字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // 创建 PivotArea 实例
            PivotArea pivotArea = new PivotArea(pivotTable);

            // 设置 PivotArea 的属性
            pivotArea.OnlyData = true;
            pivotArea.OnlyLabel = false;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.IsOutline = false;

            // 使用 Select 方法选择特定区域
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.DataAndLabel);

            // 保存工作簿
            workbook.Save("PivotAreaExample.xlsx");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


