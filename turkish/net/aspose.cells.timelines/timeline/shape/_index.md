---
title: "Timeline.Shape"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Timeline özelliği. Bu Timeline ile ilişkili TimelineShape nesnesini döndürür"
type: docs
url: /tr/net/aspose.cells.timelines/timeline/shape/
---
## Timeline.Shape property

Bu Timeline ile ilişkili [`TimelineShape`](../../../aspose.cells.drawing/timelineshape/) nesnesini döndürür.

```csharp
public TimelineShape Shape { get; }
```

### Örnekler

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
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Zaman çizelgesi için gerekli minimum veriyi ekle (tarih alanı)
            sheet.Cells["A1"].Value = "Date";
            sheet.Cells["A2"].Value = DateTime.Now.AddDays(-2);
            sheet.Cells["A3"].Value = DateTime.Now.AddDays(-1);
            sheet.Cells["A4"].Value = DateTime.Now;

            try
            {
                // Zaman çizelgesi veri kaynağı olarak hizmet verecek bir pivot tablo oluştur
                int pivotIdx = sheet.PivotTables.Add("A1:A4", "C1", "PivotTable1");
                PivotTable pivot = sheet.PivotTables[pivotIdx];
                pivot.AddFieldToArea(PivotFieldType.Row, "Date");
                pivot.RefreshData();

                // Pivot tabloyla bağlantılı bir zaman çizelgesi ekle
                int timelineIdx = sheet.Timelines.Add(pivot, 0, 0, "Date");
                Timeline timeline = sheet.Timelines[timelineIdx];

                // 'Shape' özelliğini yansıma yoluyla okumayı dene (bu sürümde mevcutsa)
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

                // Zaman çizelgesi oluşturmanın başarılı olduğunu doğrulamak için çalışma kitabını kaydedin
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

### Ayrıca Bakınız

* class [TimelineShape](../../../aspose.cells.drawing/timelineshape/)
* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


