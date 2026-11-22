---
title: "Timeline.Shape"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Timeline. تُرجع كائن TimelineShape المرتبط بهذا المخطط الزمني"
type: docs
url: /ar/net/aspose.cells.timelines/timeline/shape/
---
## Timeline.Shape property

تُرجع الكائن [`TimelineShape`](../../../aspose.cells.drawing/timelineshape/) المرتبط بهذا المخطط الزمني.

```csharp
public TimelineShape Shape { get; }
```

### أمثلة

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
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة الحد الأدنى من البيانات المطلوبة للمخطط الزمني (حقل التاريخ)
            sheet.Cells["A1"].Value = "Date";
            sheet.Cells["A2"].Value = DateTime.Now.AddDays(-2);
            sheet.Cells["A3"].Value = DateTime.Now.AddDays(-1);
            sheet.Cells["A4"].Value = DateTime.Now;

            try
            {
                // إنشاء جدول محوري سيعمل كمصدر بيانات للمخطط الزمني
                int pivotIdx = sheet.PivotTables.Add("A1:A4", "C1", "PivotTable1");
                PivotTable pivot = sheet.PivotTables[pivotIdx];
                pivot.AddFieldToArea(PivotFieldType.Row, "Date");
                pivot.RefreshData();

                // إضافة مخطط زمني مرتبط بالجدول المحوري
                int timelineIdx = sheet.Timelines.Add(pivot, 0, 0, "Date");
                Timeline timeline = sheet.Timelines[timelineIdx];

                // محاولة قراءة خاصية 'Shape' عبر الانعكاس (إذا كانت موجودة في هذا الإصدار)
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

                // احفظ المصنف للتحقق من نجاح إنشاء المخطط الزمني
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

### انظر أيضًا

* class [TimelineShape](../../../aspose.cells.drawing/timelineshape/)
* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


