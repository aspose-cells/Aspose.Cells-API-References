---
title: "WebExtensionReferenceCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebExtensionReferenceCollection. تحصل على ملحق الويب حسب الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells.webextensions/webextensionreferencecollection/item/
---
## WebExtensionReferenceCollection indexer

يحصل على امتداد الويب حسب الفهرس المحدد.

```csharp
public WebExtensionReference this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس. |

### قيمة الإرجاع

ملحق الويب

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionReferenceCollectionPropertyItemDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء WebExtensionReferenceCollection جديد
                WebExtensionReferenceCollection references = new WebExtensionReferenceCollection();
                
                // إضافة مرجع جديد لامتداد الويب
                int index = references.Add();
                
                // الوصول إلى خاصية Item (للقراءة فقط) للحصول على المرجع عند الفهرس المحدد
                WebExtensionReference reference = references[index];
                
                // عرض معلومات حول المرجع المسترجع
                Console.WriteLine($"Retrieved web extension reference at index: {index}");
                Console.WriteLine($"Reference type: {reference.GetType().Name}");
                
                // ملاحظة: خاصية Item للقراءة فقط، لذا نعرض فقط الحصول على قيمتها
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating Item property: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [WebExtensionReference](../../webextensionreference/)
* class [WebExtensionReferenceCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


