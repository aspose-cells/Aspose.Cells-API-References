---
title: "WebExtension.Id"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebExtension. يحصل على ويضبط المعرف الفريد لمثيل إضافة Office في المستند الحالي"
type: docs
url: /ar/net/aspose.cells.webextensions/webextension/id/
---
## WebExtension.Id property

يحصل ويضبط المعرف الفريد لنسخة مكوّن Office في المستند الحالي.

```csharp
public string Id { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyIdDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // الحصول على مجموعة امتدادات الويب من المصنف
                var webExtensions = workbook.Worksheets.WebExtensions;
                
                // إضافة امتداد ويب جديد (سيتم إنشاؤه مع المعلمات المطلوبة)
                int index = webExtensions.Add();
                WebExtension webExtension = webExtensions[index];
                
                // ضبط خاصية Id (لأنها للقراءة والكتابة)
                webExtension.Id = "SampleAddin123";
                
                // عرض القيمة الحالية لخاصية Id
                Console.WriteLine($"WebExtension Id: {webExtension.Id}");
                
                // تعديل خاصية Id لإظهار أنها قابلة للكتابة
                webExtension.Id = "UpdatedAddin456";
                Console.WriteLine($"Updated WebExtension Id: {webExtension.Id}");
                
                // احفظ المصنف
                workbook.Save("WebExtensionIdDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


