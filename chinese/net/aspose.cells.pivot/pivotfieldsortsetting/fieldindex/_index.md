---
title: "PivotFieldSortSetting.FieldIndex"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotFieldSortSetting 属性。表示用于排序的字段索引。1 表示按标签对 PivotField 进行排序，其他值表示按数据字段进行排序"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfieldsortsetting/fieldindex/
---
## PivotFieldSortSetting.FieldIndex property

表示用于排序的字段索引。-1 表示按标签对 PivotField 进行排序，其他值表示按数据字段进行排序。

```csharp
[Obsolete("Use PivotFieldSortSetting.SortBy property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int FieldIndex { get; set; }
```

### 备注

注意：此属性已过时。请改用 PivotFieldSortSetting.SortBy 属性。此方法将在自 2026 年 9 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSortSettingPropertyFieldIndexDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为数据透视表添加示例数据
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["B4"].Value = 8;

            // 创建数据透视表
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // 获取透视字段排序设置
            PivotFieldSortSetting sortSetting = pivotTable.RowFields[0].SortSetting;

            // 显示当前 FieldIndex 值
            Console.WriteLine("Current FieldIndex value: " + sortSetting.FieldIndex);

            // 注意：FieldIndex 为只读，且 PivotFieldSortSetting 不能直接实例化
            // 因为它没有公共构造函数。我们只能使用现有实例
            // 从透视字段的 SortSetting 属性获取。

            // 刷新数据透视表以应用更改
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // 保存结果
            workbook.Save("PivotFieldSortSettingFieldIndexDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


