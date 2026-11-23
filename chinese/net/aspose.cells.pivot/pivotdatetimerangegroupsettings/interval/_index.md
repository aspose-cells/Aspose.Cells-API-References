---
title: "PivotDateTimeRangeGroupSettings.Interval"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotDateTimeRangeGroupSettings 属性。获取组的内部"
type: docs
url: /zh/net/aspose.cells.pivot/pivotdatetimerangegroupsettings/interval/
---
## PivotDateTimeRangeGroupSettings.Interval property

获取组的内部信息。

```csharp
public double Interval { get; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotDateTimeRangeGroupSettingsPropertyIntervalDemo
    {
        public static void Run()
        {
            // 创建工作簿
            Workbook workbook = new Workbook();
            
            // 添加包含示例数据的工作表
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            
            // 添加示例日期数据
            dataSheet.Cells["A1"].PutValue("Date");
            dataSheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-5));
            dataSheet.Cells["A3"].PutValue(DateTime.Now.AddDays(-4));
            dataSheet.Cells["A4"].PutValue(DateTime.Now.AddDays(-3));
            dataSheet.Cells["A5"].PutValue(DateTime.Now.AddDays(-2));
            dataSheet.Cells["A6"].PutValue(DateTime.Now.AddDays(-1));
            dataSheet.Cells["A7"].PutValue(DateTime.Now);

            // 添加数据透视表工作表
            Worksheet pivotSheet = workbook.Worksheets.Add("Pivot");
            
            // 添加透视表
            int pivotIndex = pivotSheet.PivotTables.Add(
                "=Data!A1:A7", 
                "A1", 
                "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];

            // 将日期字段添加到行区域
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotField dateField = pivotTable.RowFields[0];

            // 按天分组，间隔为 2
            dateField.GroupBy(1, false);
            PivotDateTimeRangeGroupSettings groupSettings = 
                (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;
            
            // 由于 Interval 为只读，我们需要在分组时设置它
            // 间隔实际上在 GroupBy 方法的参数中设置
            // 这里我们仅验证间隔值
            Console.WriteLine($"Grouping interval: {groupSettings.Interval} days");

            // 保存工作簿
            workbook.Save("PivotDateTimeGroupingDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotDateTimeRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


