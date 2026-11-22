---
title: "JsonLoadOptions.StartCell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية JsonLoadOptions. الحصول على وتعيين الخلية البداية"
type: docs
url: /ar/net/aspose.cells/jsonloadoptions/startcell/
---
## JsonLoadOptions.StartCell property

يحصل على خلية البداية ويضبطها.

```csharp
public string StartCell { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonLoadOptionsPropertyStartCellDemo
    {
        public static void Run()
        {
            // إنشاء خيارات تحميل JSON باستخدام خاصية StartCell
            JsonLoadOptions options = new JsonLoadOptions
            {
                StartCell = "B3" // JSON data will start from cell B3
            };

            // إنشاء دفتر عمل من ملف JSON مع الخيارات
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("Header");
            
            // إنشاء ملف JSON تجريبي
            System.IO.File.WriteAllText("data.json", "{\"Name\":\"John\",\"Age\":30,\"City\":\"New York\"}");
            
            // تحميل بيانات JSON إلى دفتر العمل
            workbook = new Workbook("data.json", options);

            // احفظ المصنف
            workbook.Save("JsonStartCellDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


