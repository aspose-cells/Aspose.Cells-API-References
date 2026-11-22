---
title: "SmartTagProperty.Value"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SmartTagProperty. تحصل وتضبط قيمة الخاصية"
type: docs
url: /ar/net/aspose.cells.markup/smarttagproperty/value/
---
## SmartTagProperty.Value property

يحصل ويضبط قيمة الخاصية.

```csharp
public string Value { get; set; }
```

### أمثلة

```csharp
using Aspose.Cells.Markup;
using System;

namespace AsposeCellsExamples
{
    public class SmartTagPropertyPropertyValueDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء نسخة من SmartTagProperty باستخدام المُنشئ غير العام
                var property = (SmartTagProperty)Activator.CreateInstance(typeof(SmartTagProperty), true);

                // ضبط اسم وقيمة الخاصية
                property.Name = "Category";
                property.Value = "Finance";

                // عرض قيم الخصائص
                Console.WriteLine($"SmartTagProperty Name : {property.Name}");
                Console.WriteLine($"SmartTagProperty Value: {property.Value}");
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

* class [SmartTagProperty](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


