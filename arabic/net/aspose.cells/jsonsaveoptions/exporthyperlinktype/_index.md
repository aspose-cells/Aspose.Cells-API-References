---
title: "JsonSaveOptions.ExportHyperlinkType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية JsonSaveOptions. تمثل نوع تصدير الارتباط التشعبي إلى json"
type: docs
url: /ar/net/aspose.cells/jsonsaveoptions/exporthyperlinktype/
---
## JsonSaveOptions.ExportHyperlinkType property

يمثل نوع تصدير الروابط التشعبية إلى JSON.

```csharp
public JsonExportHyperlinkType ExportHyperlinkType { get; set; }
```

### ملاحظات

القيمة الافتراضية هي DisplayString؛

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Json;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportHyperlinkTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة ارتباط تشعبي إلى الخلية A1
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // تعيين خيارات التصدير لـ JSON
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.HtmlString;
            
            // حفظ المصنف إلى JSON
            string outputPath = "output.json";
            workbook.Save(outputPath, saveOptions);
            
            // التحقق من أن المخرجات تحتوي على الارتباط التشعبي
            string jsonContent = File.ReadAllText(outputPath);
            Console.WriteLine("JSON content contains hyperlink: " + 
                jsonContent.Contains("https://www.aspose.com"));
        }
    }
}
```

### انظر أيضًا

* enum [JsonExportHyperlinkType](../../../aspose.cells.json/jsonexporthyperlinktype/)
* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


