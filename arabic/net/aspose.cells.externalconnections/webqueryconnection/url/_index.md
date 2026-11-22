---
title: "WebQueryConnection.Url"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebQueryConnection. عنوان URL لاستخدامه لتحديث البيانات الخارجية"
type: docs
url: /ar/net/aspose.cells.externalconnections/webqueryconnection/url/
---
## WebQueryConnection.Url property

URL لاستخدامه لتحديث البيانات الخارجية.

```csharp
public string Url { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyUrlDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء اتصال استعلام ويب عن طريق إضافته إلى المجموعة
            // من المحتمل أن تقوم المجموعة بإنشاء وإرجاع كائن الاتصال
            WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[workbook.DataConnections.Count];

            // تعيين عنوان URL الأولي لاستعلام الويب
            connection.Url = "https://example.com/data.html";
            Console.WriteLine("Initial URL: " + connection.Url);

            // تغيير عنوان URL إلى مصدر مختلف
            connection.Url = "https://example.com/updated-data.xml";
            Console.WriteLine("Updated URL: " + connection.Url);

            // تكوين الاتصال لتحليل بيانات XML
            connection.IsXml = true;

            // تحديث اتصال البيانات (عادةً ما يسترجع البيانات من عنوان URL)
            // ملاحظة: الوصول الفعلي إلى الويب سيتطلب اتصالًا بالشبكة
            // workbook.RefreshAllConnections();

            // حفظ المصنف مع اتصال استعلام الويب
            workbook.Save("WebQueryConnectionUrlDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


