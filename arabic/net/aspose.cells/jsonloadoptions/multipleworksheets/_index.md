---
title: "JsonLoadOptions.MultipleWorksheets"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية JsonLoadOptions. تشير إلى ما إذا كان يتم استيراد كل سمة من كائن JsonObject كورقة عمل واحدة عندما تكون جميع العقد الفرعية عقد مصفوفة"
type: docs
url: /ar/net/aspose.cells/jsonloadoptions/multipleworksheets/
---
## JsonLoadOptions.MultipleWorksheets property

يشير إلى ما إذا كان يتم استيراد كل سمة من كائن JsonObject كورقة عمل واحدة عندما تكون جميع العقد الفرعية عقد مصفوفة.

```csharp
public bool MultipleWorksheets { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonLoadOptionsPropertyMultipleWorksheetsDemo
    {
        public static void Run()
        {
            // إنشاء خيارات تحميل JSON مع تمكين MultipleWorksheets
            JsonLoadOptions options = new JsonLoadOptions { MultipleWorksheets = true };
            
            // تحميل ملف JSON إلى دفتر العمل باستخدام الخيارات المحددة
            Workbook workbook = new Workbook("example.json", options);
            
            // الوصول إلى البيانات من ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // عرض بعض القيم التجريبية من JSON المحمَّل
            Console.WriteLine("D5 cell value: " + cells["D5"].StringValue);
            Console.WriteLine("E5 cell value: " + cells["E5"].StringValue);
            Console.WriteLine("D7 cell value: " + cells["D7"].StringValue);
            Console.WriteLine("B14 cell value: " + cells["B14"].StringValue);
        }
    }
}
```

### انظر أيضًا

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


