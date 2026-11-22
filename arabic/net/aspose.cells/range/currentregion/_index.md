---
title: "Range.CurrentRegion"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Range. تُرجع كائن Range يمثل المنطقة الحالية. المنطقة الحالية هي نطاق يحده أي تركيبة من الصفوف الفارغة والأعمدة الفارغة"
type: docs
url: /ar/net/aspose.cells/range/currentregion/
---
## Range.CurrentRegion property

يرجع كائن Range يمثل المنطقة الحالية. المنطقة الحالية هي نطاق محاط بأي تركيبة من الصفوف الفارغة والأعمدة الفارغة.

```csharp
public Range CurrentRegion { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangePropertyCurrentRegionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // املأ البيانات ببعض الخلايا الفارغة لإنشاء مناطق
            worksheet.Cells["A1"].PutValue("Region 1");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue("Data 2");
            worksheet.Cells["A4"].PutValue("Data 3");
            
            // اترك الصف 5 فارغًا لفصل المناطق
            
            worksheet.Cells["A6"].PutValue("Region 2");
            worksheet.Cells["A7"].PutValue("Data 4");
            worksheet.Cells["B7"].PutValue("Data 5");
            worksheet.Cells["A8"].PutValue("Data 6");

            // احصل على خلية في المنطقة الأولى وحولها إلى Range
            Aspose.Cells.Range cellInRegion1 = worksheet.Cells.CreateRange("A2", "A2");
            Aspose.Cells.Range currentRegion1 = cellInRegion1.CurrentRegion;
            
            Console.WriteLine("CurrentRegion for A2: " + currentRegion1.Address);
            Console.WriteLine("Row count in region: " + currentRegion1.RowCount);
            Console.WriteLine("Column count in region: " + currentRegion1.ColumnCount);

            // احصل على خلية في المنطقة الثانية وحولها إلى Range
            Aspose.Cells.Range cellInRegion2 = worksheet.Cells.CreateRange("B7", "B7");
            Aspose.Cells.Range currentRegion2 = cellInRegion2.CurrentRegion;
            
            Console.WriteLine("\nCurrentRegion for B7: " + currentRegion2.Address);
            Console.WriteLine("Row count in region: " + currentRegion2.RowCount);
            Console.WriteLine("Column count in region: " + currentRegion2.ColumnCount);

            // طبق التنسيق على المنطقة الحالية بأكملها
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;
            
            currentRegion1.SetStyle(style);

            // احفظ المصنف
            workbook.Save("RangePropertyCurrentRegionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


