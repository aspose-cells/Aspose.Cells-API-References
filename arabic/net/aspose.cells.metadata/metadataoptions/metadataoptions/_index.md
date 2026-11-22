---
title: "MetadataOptions.MetadataOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ MetadataOptions. ينشئ خيارات لتحميل البيانات الوصفية"
type: docs
url: /ar/net/aspose.cells.metadata/metadataoptions/metadataoptions/
---
## MetadataOptions constructor

ينشئ خيارات تحميل البيانات الوصفية.

```csharp
public MetadataOptions(MetadataType metadataType)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| metadataType | MetadataType | نوع البيانات الوصفية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using System;

    public class MetadataOptionsMethodCtorWithMetadataTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // استدعاء طريقة #ctor مع معامل MetadataType
                MetadataOptions options = new MetadataOptions(MetadataType.Encryption);
                
                // عيّن الخصائص الإضافية
                options.Password = "test123";
                options.KeyLength = 128;
                
                // عرض الخيارات التي تم إنشاؤها
                Console.WriteLine($"MetadataType: {options.MetadataType}");
                Console.WriteLine($"Password set: {!string.IsNullOrEmpty(options.Password)}");
                Console.WriteLine($"KeyLength: {options.KeyLength}");

                // استخدام الخيارات عند تحميل البيانات الوصفية (مثال)
                // عادةً ما يتم استخدام هذا مع LoadOptions عند فتح ملف
                // ملاحظة: حاول الكود الأصلي تعيين MetadataOptions مباشرةً على LoadOptions،
                // لكن فئة LoadOptions لا تحتوي على هذه الخاصية في التعريف المقدم.
                // سنبقي فقط جزء إنشاء الخيارات لأن الاستخدام مع LoadOptions
                // ليس ممكنًا مع تعريف API الحالي.
                
                Console.WriteLine("MetadataOptions created successfully with MetadataType parameter");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating MetadataOptions: {ex.Message}");
            }
            
            // احفظ المصنف (على الرغم من أن خيارات البيانات الوصفية لن تؤثر على هذا المصنف الفارغ)
            workbook.Save("MetadataOptionsCtorDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [MetadataType](../../metadatatype/)
* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


