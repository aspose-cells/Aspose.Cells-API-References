---
title: "类 PivotDateTimeRangeGroupSettings"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Pivot.PivotDateTimeRangeGroupSettings 类。表示按日期时间范围分组的字段"
type: docs
url: /zh/net/aspose.cells.pivot/pivotdatetimerangegroupsettings/
---
## PivotDateTimeRangeGroupSettings class

表示按日期时间范围分组的字段。

```csharp
public class PivotDateTimeRangeGroupSettings : PivotFieldGroupSettings
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [End](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/end/) { get; } | 获取组的结束日期时间。 |
| [GroupByTypes](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/groupbytypes/) { get; } | 获取按日期时间的分组类型。 |
| [Interval](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/interval/) { get; } | 获取组的内部信息。 |
| [Start](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/start/) { get; } | 获取组的开始日期时间。 |
| override [Type](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/type/) { get; } | 获取数据时间组类型。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [IsGroupedBy](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/isgroupedby/)(PivotGroupByType) | 检查字段是否按该类型分组。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotDateTimeRangeGroupSettingsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // 添加带日期的示例数据
                worksheet.Cells["A1"].PutValue("Date");
                worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
                worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
                worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["B2"].PutValue(10);
                worksheet.Cells["B3"].PutValue(20);
                worksheet.Cells["B4"].PutValue(30);

                // 创建数据透视表
                int pivotIndex = worksheet.PivotTables.Add("=A1:B4", "E3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // 向数据透视表添加字段
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // 按月份对日期字段进行分组
                PivotField dateField = pivotTable.RowFields[0];
                DateTime startDate = new DateTime(2023, 1, 1);
                DateTime endDate = new DateTime(2023, 12, 31);
                dateField.GroupBy(startDate, endDate, new PivotGroupByType[] { PivotGroupByType.Months }, 1, false);

                // 获取分组设置
                PivotDateTimeRangeGroupSettings groupSettings = (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;

                // 显示分组设置属性
                Console.WriteLine($"Group Type: {groupSettings.Type}");
                Console.WriteLine($"Start Date: {groupSettings.Start}");
                Console.WriteLine($"End Date: {groupSettings.End}");
                Console.WriteLine($"Interval: {groupSettings.Interval}");
                Console.WriteLine($"Group By Types: {string.Join(", ", groupSettings.GroupByTypes)}");

                // 检查是否按月份分组
                bool isGroupedByMonths = groupSettings.IsGroupedBy(PivotGroupByType.Months);
                Console.WriteLine($"Is grouped by months: {isGroupedByMonths}");

                // 保存工作簿
                workbook.Save("PivotDateTimeRangeGroupSettingsDemo.xlsx");
                Console.WriteLine("PivotDateTimeRangeGroupSettings demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in PivotDateTimeRangeGroupSettings demo: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [PivotFieldGroupSettings](../pivotfieldgroupsettings/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


