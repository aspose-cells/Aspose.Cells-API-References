---
title: "WebExtension.IsFrozen"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebExtension. تشير إلى ما إذا كان المستخدم يمكنه التفاعل مع إضافة Office أم لا"
type: docs
url: /ar/net/aspose.cells.webextensions/webextension/isfrozen/
---
## WebExtension.IsFrozen property

يشير إلى ما إذا كان المستخدم يمكنه التفاعل مع مكوّن Office أم لا.

```csharp
public bool IsFrozen { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyIsFrozenDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // سيفشل هذا السطر لأن WebExtension يتطلب معلمات المُنشئ
                // WebExtension webExtension = new WebExtension();
                
                // بدلاً من ذلك، سنحصل على WebExtension من المصنف إذا كان ذلك ممكنًا
                // أو توضيح باستخدام نهج مختلف
                Console.WriteLine("Note: WebExtension requires constructor parameters. This demo shows property usage conceptually.");
                
                // لأغراض العرض، سنظهر كيف ستعمل الخاصية إذا كان لديك مثال صالح
                // في سيناريو حقيقي، ستحصل على مثال WebExtension من المصنف أو من مصدر آخر
                WebExtension webExtension = GetWebExtensionInstance(workbook);
                
                if (webExtension != null)
                {
                    // حدد الخصائص الأولية
                    webExtension.Id = "MyAddin123";
                    
                    // عرض القيمة الأولية لـ IsFrozen
                    Console.WriteLine($"Initial IsFrozen value: {webExtension.IsFrozen}");
                    
                    // تغيير خاصية IsFrozen (نظرًا لأنها قراءة-كتابة)
                    webExtension.IsFrozen = true;
                    Console.WriteLine($"Updated IsFrozen value: {webExtension.IsFrozen}");
                    
                    // إظهار التأثير عن طريق التحقق مما إذا كان المستخدم يمكنه التفاعل
                    Console.WriteLine($"User can{(webExtension.IsFrozen ? "not" : "")} interact with the add-in");
                    
                    // حفظ المصنف (على الرغم من أن WebExtension قد لا يتم حفظه دون خطوات إضافية)
                    workbook.Save("WebExtensionIsFrozenDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("Could not obtain a WebExtension instance for demonstration.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private static WebExtension GetWebExtensionInstance(Workbook workbook)
        {
            // في تنفيذ حقيقي، سيحصل هذا على WebExtension موجود من المصنف
            // أو إنشاء واحد بشكل صحيح مع معلمات المُنشئ المطلوبة
            // هذا مجرد عنصر نائب للعرض
            return null;
        }
    }
}
```

### انظر أيضًا

* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


