---
title: "ExternalLink.OriginalDataSource"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalLink. تمثل مصدر البيانات المخزن للارتباط الخارجي"
type: docs
url: /ar/net/aspose.cells/externallink/originaldatasource/
---
## ExternalLink.OriginalDataSource property

يمثل مصدر البيانات المخزن للارتباط الخارجي.

```csharp
public string OriginalDataSource { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyOriginalDataSourceDemo
    {
        public static void Run()
        {
            // إنشاء مصنف يحتوي على روابط خارجية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة ارتباط خارجي
            worksheet.Cells["A1"].Formula = "='https://arcusventures.sharepoint.com/Fund II/[example.xlsx]Sheet1'!A1";
            
            // تعديل مسارات الارتباط الخارجي
            for (int i = 0; i < workbook.Worksheets.ExternalLinks.Count; i++)
            {
                string originalLink = workbook.Worksheets.ExternalLinks[i].OriginalDataSource;
                string modifiedLink = originalLink.Replace(
                    @"https://arcusventures.sharepoint.com/Fund II/", 
                    @"/sites/shared/shared documents/Fund II/");
                
                workbook.Worksheets.ExternalLinks[i].OriginalDataSource = modifiedLink;
            }
            
            // تحقق من التغييرات
            foreach (ExternalLink link in workbook.Worksheets.ExternalLinks)
            {
                Console.WriteLine("Modified Link: " + link.OriginalDataSource);
            }
        }
    }
}
```

### انظر أيضًا

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


