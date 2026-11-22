---
title: "الفئة SmartTagProperty"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Markup.SmartTagProperty. تمثل خاصية الـ smart tag للخلية"
type: docs
url: /ar/net/aspose.cells.markup/smarttagproperty/
---
## SmartTagProperty class

يمثل خاصية علامة الخلية الذكية.

```csharp
public class SmartTagProperty
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Name](../../aspose.cells.markup/smarttagproperty/name/) { get; set; } | يحصل ويضبط اسم الخاصية. |
| [Value](../../aspose.cells.markup/smarttagproperty/value/) { get; set; } | يحصل ويضبط قيمة الخاصية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Markup;
    using System;

    public class MarkupClassSmartTagPropertyDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء نسخة من SmartTagProperty باستخدام الانعكاس لأن المُنشئ غير عام
                var smartTagProperty = (SmartTagProperty)Activator.CreateInstance(typeof(SmartTagProperty), true);

                // ضبط خصائص Name و Value
                smartTagProperty.Name = "DocumentType";
                smartTagProperty.Value = "FinancialReport";

                // عرض قيم الخصائص
                Console.WriteLine($"SmartTagProperty Name: {smartTagProperty.Name}");
                Console.WriteLine($"SmartTagProperty Value: {smartTagProperty.Value}");

                // توضيح تعديل الخصائص
                smartTagProperty.Name = "Status";
                smartTagProperty.Value = "Approved";

                Console.WriteLine($"Updated SmartTagProperty Name: {smartTagProperty.Name}");
                Console.WriteLine($"Updated SmartTagProperty Value: {smartTagProperty.Value}");

                Console.WriteLine("SmartTagProperty demonstration completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SmartTagProperty: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


