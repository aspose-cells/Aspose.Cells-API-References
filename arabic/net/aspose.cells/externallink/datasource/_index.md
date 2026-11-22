---
title: "ExternalLink.DataSource"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalLink. تمثل مصدر البيانات للارتباط الخارجي"
type: docs
url: /ar/net/aspose.cells/externallink/datasource/
---
## ExternalLink.DataSource property

يمثل مصدر البيانات للارتباط الخارجي.

```csharp
public string DataSource { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyDataSourceDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف ورقة عمل
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء ارتباط خارجي إلى مصنف آخر
            worksheet.Cells["A1"].Formula = "='[external.xlsx]Sheet1'!A1";
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
            
            // تحميل المصنف المحفوظ للتحقق من الروابط الخارجية
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            
            // الوصول إلى خاصية DataSource للارتباط الخارجي
            if (loadedWorkbook.Worksheets.ExternalLinks.Count > 0)
            {
                string dataSource = loadedWorkbook.Worksheets.ExternalLinks[0].DataSource;
                Console.WriteLine("External link data source: " + dataSource);
            }
        }
    }
}
```

### انظر أيضًا

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


