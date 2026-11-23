---
title: "Timeline.Shape"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Timeline 属性。返回与此 Timeline 关联的 TimelineShape 对象"
type: docs
url: /zh/net/aspose.cells.timelines/timeline/shape/
---
## Timeline.Shape property

返回与此 Timeline 关联的 [`TimelineShape`](../../../aspose.cells.drawing/timelineshape/) 对象。

```csharp
public TimelineShape Shape { get; }
```

### 示例

```csharp
using System;
using System.Reflection;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Timelines;

namespace AsposeCellsExamples
{
    public class TimelinePropertyShapeDemo
    {
        public static void Run()
        {
            // 创建新工作簿并获取第一个工作表
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // 添加时间线所需的最少数据（日期字段）
            sheet.Cells["A1"].Value = "Date";
            sheet.Cells["A2"].Value = DateTime.Now.AddDays(-2);
            sheet.Cells["A3"].Value = DateTime.Now.AddDays(-1);
            sheet.Cells["A4"].Value = DateTime.Now;

            try
            {
                // 创建一个透视表，用作时间轴的数据源
                int pivotIdx = sheet.PivotTables.Add("A1:A4", "C1", "PivotTable1");
                PivotTable pivot = sheet.PivotTables[pivotIdx];
                pivot.AddFieldToArea(PivotFieldType.Row, "Date");
                pivot.RefreshData();

                // 添加一个链接到透视表的时间轴
                int timelineIdx = sheet.Timelines.Add(pivot, 0, 0, "Date");
                Timeline timeline = sheet.Timelines[timelineIdx];

                // 尝试通过反射读取 'Shape' 属性（如果此版本中存在）
                PropertyInfo shapeProp = typeof(Timeline).GetProperty("Shape", BindingFlags.Public | BindingFlags.Instance);
                if (shapeProp != null)
                {
                    object shapeValue = shapeProp.GetValue(timeline);
                    Console.WriteLine("Shape property value: " + (shapeValue ?? "null"));
                }
                else
                {
                    Console.WriteLine("The Timeline class does not expose a 'Shape' property in this version.");
                }

                // 保存工作簿以验证时间轴创建是否成功
                workbook.Save("TimelineShapeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [TimelineShape](../../../aspose.cells.drawing/timelineshape/)
* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


