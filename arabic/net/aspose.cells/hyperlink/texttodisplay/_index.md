---
title: "Hyperlink.TextToDisplay"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Hyperlink. تمثل النص الذي سيُعرض للارتباط التشعبي المحدد. القيمة الافتراضية هي عنوان الارتباط التشعبي"
type: docs
url: /ar/net/aspose.cells/hyperlink/texttodisplay/
---
## Hyperlink.TextToDisplay property

يمثل النص الذي سيُعرض للرابط التشعبي المحدد. القيمة الافتراضية هي عنوان الرابط التشعبي.

```csharp
public string TextToDisplay { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyTextToDisplayDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف ارتباطات تشعبية باستخدام خاصية TextToDisplay
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;
            
            // أضف أول ارتباط تشعبي بنص عرض مخصص
            int index1 = hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            hyperlinks[index1].TextToDisplay = "Visit Aspose Website";
            
            // أضف الارتباط التشعبي الثاني مع نص عرض مخصص
            int index2 = hyperlinks.Add("A2", 1, 1, "https://docs.aspose.com");
            hyperlinks[index2].TextToDisplay = "Aspose Documentation";
            
            // أضف الارتباط التشعبي الثالث مع مرجع الخلية كنص عرض
            int index3 = hyperlinks.Add("A3", 1, 1, "Sheet2!B5");
            hyperlinks[index3].TextToDisplay = "Go to Sheet2!B5";
            
            // احفظ المصنف
            string outputPath = "HyperlinkTextToDisplayDemo.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with hyperlinks using TextToDisplay property: " + outputPath);
        }
    }
}
```

### انظر أيضًا

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


