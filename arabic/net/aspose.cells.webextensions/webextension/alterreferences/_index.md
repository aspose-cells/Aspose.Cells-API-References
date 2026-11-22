---
title: "WebExtension.AlterReferences"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebExtension. يحصل على قائمة بالمراجع المعدلة"
type: docs
url: /ar/net/aspose.cells.webextensions/webextension/alterreferences/
---
## WebExtension.AlterReferences property

يحصل على قائمة بالمراجع المعدلة.

```csharp
public WebExtensionReferenceCollection AlterReferences { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyAlterReferencesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // الحصول على مجموعة امتدادات الويب من المصنف
                var webExtensions = workbook.Worksheets.WebExtensions;
                
                // إضافة امتداد ويب جديد
                int index = webExtensions.Add();
                WebExtension webExtension = webExtensions[index];
                
                // الوصول إلى خاصية AlterReferences (للقراءة فقط)
                WebExtensionReferenceCollection alterReferences = webExtension.AlterReferences;
                
                // عرض معلومات حول مراجع التعديل
                Console.WriteLine($"Number of alter references: {alterReferences.Count}");
                
                // إضافة مرجع تعديل جديد (يوضح استخدام المجموعة)
                int newRefIndex = alterReferences.Add();
                Console.WriteLine($"Added new alter reference at index: {newRefIndex}");
                
                // عرض العدد المحدث
                Console.WriteLine($"Updated number of alter references: {alterReferences.Count}");
                
                // احفظ المصنف
                workbook.Save("WebExtensionAlterReferencesDemo.xlsx");
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

* class [WebExtensionReferenceCollection](../../webextensionreferencecollection/)
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


