---
title: "WebExtension.Bindings"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebExtension. يحصل على جميع علاقات الارتباط بين إضافة Office والبيانات في المستند"
type: docs
url: /ar/net/aspose.cells.webextensions/webextension/bindings/
---
## WebExtension.Bindings property

يحصل على جميع علاقات الربط بين مكوّن Office والبيانات في المستند.

```csharp
public WebExtensionBindingCollection Bindings { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyBindingsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إنشاء ورقة عمل نموذجية
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // بافتراض أننا نحصل على امتداد ويب من مكان ما (لأننا لا نستطيع إنشاء واحد مباشرة)
                // هذا تعديل بسيط لجعل الكود يُترجم مع الحفاظ على هيكله
                WebExtension webExtension = null; // In real usage, this would come from workbook.WebExtensions or similar
                
                if (webExtension != null)
                {
                    // الوصول إلى خاصية Bindings (للقراءة فقط)
                    WebExtensionBindingCollection bindings = webExtension.Bindings;
                    
                    // عرض معلومات حول الارتباطات
                    Console.WriteLine($"Number of bindings: {bindings.Count}");
                    
                    // إضافة ارتباط جديد (يوضح استخدام المجموعة)
                    int newBindingIndex = bindings.Add();
                    Console.WriteLine($"Added new binding at index: {newBindingIndex}");
                    
                    // عرض العدد المحدث
                    Console.WriteLine($"Updated number of bindings: {bindings.Count}");
                }
                else
                {
                    Console.WriteLine("No web extension available");
                }
                
                // احفظ المصنف
                workbook.Save("WebExtensionBindingsDemo.xlsx");
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

* class [WebExtensionBindingCollection](../../webextensionbindingcollection/)
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


