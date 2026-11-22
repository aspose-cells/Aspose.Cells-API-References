---
title: "JsonSaveOptions.JsonSaveOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ JsonSaveOptions. ينشئ خيارات لحفظ ملف json"
type: docs
url: /ar/net/aspose.cells/jsonsaveoptions/jsonsaveoptions/
---
## JsonSaveOptions constructor

ينشئ خيارات لحفظ ملف JSON.

```csharp
public JsonSaveOptions()
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // بيانات عينة لتصديرها كـ JSON
            workbook.Worksheets[0].Cells["A1"].PutValue("Name");
            workbook.Worksheets[0].Cells["B1"].PutValue("Age");
            workbook.Worksheets[0].Cells["A2"].PutValue("John");
            workbook.Worksheets[0].Cells["B2"].PutValue(30);
            
            // تهيئة JsonSaveOptions باستخدام المنشئ
            JsonSaveOptions options = new JsonSaveOptions();
            
            // تعيين خيارات تصدير JSON
            options.ExportNestedStructure = true;
            options.SkipEmptyRows = true;
            options.ValidateMergedAreas = true;
            
            // حفظ دفتر العمل باستخدام خيارات JSON
            string outputPath = "output.json";
            workbook.Save(outputPath, options);
            
            Console.WriteLine("JSON file saved successfully with options.");
        }
    }
}
```

### انظر أيضًا

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


