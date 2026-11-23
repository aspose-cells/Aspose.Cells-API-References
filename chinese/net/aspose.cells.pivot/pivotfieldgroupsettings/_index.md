---
title: "类 PivotFieldGroupSettings"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Pivot.PivotFieldGroupSettings 类。表示透视字段的分组设置"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfieldgroupsettings/
---
## PivotFieldGroupSettings class

表示透视字段的分组设置。

```csharp
public class PivotFieldGroupSettings
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [PivotFieldGroupSettings](pivotfieldgroupsettings/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| virtual [Type](../../aspose.cells.pivot/pivotfieldgroupsettings/type/) { get; } | 获取透视字段的分组类型。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldGroupSettingsDemo
    {
        public static void PivotFieldGroupSettingsExample()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 向工作表添加一些数据
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[3, 0].Value = "Cherry";
            worksheet.Cells[4, 0].Value = "Date";

            worksheet.Cells[0, 1].Value = "Amount";
            worksheet.Cells[1, 1].Value = 50;
            worksheet.Cells[2, 1].Value = 60;
            worksheet.Cells[3, 1].Value = 70;
            worksheet.Cells[4, 1].Value = 80;

            // 向工作表添加透视表
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // 向数据透视表添加字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount

            // 访问行字段
            PivotField rowField = pivotTable.RowFields[0];
            rowField.GroupBy(new CustomPiovtFieldGroupItem[] { new CustomPiovtFieldGroupItem("TestItemGroup", new int[] { 0, 1 }) }, true);

            // 访问行字段的分组设置
            PivotFieldGroupSettings groupSettings = rowField.GroupSettings;

            // 显示透视字段的分组类型
            Console.WriteLine("Group Type: " + groupSettings.Type);

            // 保存工作簿
            workbook.Save("PivotFieldGroupSettingsExample.xlsx");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


