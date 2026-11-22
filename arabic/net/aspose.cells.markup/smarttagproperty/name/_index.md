---
title: "SmartTagProperty.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SmartTagProperty. تحصل وتضبط اسم الخاصية"
type: docs
url: /ar/net/aspose.cells.markup/smarttagproperty/name/
---
## SmartTagProperty.Name property

يحصل ويضبط اسم الخاصية.

```csharp
public string Name { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Markup;
    using System;
    using System.Reflection;

    public class SmartTagPropertyPropertyNameDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء نسخة من SmartTagProperty باستخدام الانعكاس لأن المُنشئ غير عام
                var property = (SmartTagProperty)Activator.CreateInstance(typeof(SmartTagProperty), true);

                // عيّن خاصية Name
                property.Name = "Department";

                // اعرض القيمة الحالية لخاصية Name
                Console.WriteLine("SmartTagProperty Name: " + property.Name);

                // إظهار تغيير خاصية Name
                property.Name = "Project";
                Console.WriteLine("Updated SmartTagProperty Name: " + property.Name);

                // أظهر أن الخاصية يمكن قراءتها وتعديلها
                Console.WriteLine("Name property demonstration completed successfully");
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


