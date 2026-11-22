---
title: "LoadOptions.Region"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LoadOptions. تحصل أو تعين الإعدادات الإقليمية المستخدمة للمصنف الذي سيتم تحميله"
type: docs
url: /ar/net/aspose.cells/loadoptions/region/
---
## LoadOptions.Region property

يحصل أو يضبط الإعدادات الإقليمية المستخدمة للمصنف الذي سيتم تحميله.

```csharp
public CountryCode Region { get; set; }
```

### ملاحظات

قد تُستخدم الإعدادات الإقليمية لتهيئة بعض الميزات للمصنف مثل الخطوط والسمات وما إلى ذلك. بالنسبة لتنسيقات الملفات النصية، مثل CSV و HTML، ...، ستُستخدم الإعدادات الإقليمية أيضًا لاكتشاف تنسيقات الأرقام وتحويل القيم النصية إلى قيم رقمية أو تاريخية للخلايا. سيتم الاحتفاظ بهذا الإعداد للمصنف المُنشأ لاحقًا، أي أن [`Region`](../../workbooksettings/region/) للمصنف سيستخدم نفس المنطقة مع هذه الخاصية.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyRegionDemo
    {
        public static void Run()
        {
            // إنشاء خيارات التحميل لملف HTML
            LoadOptions loadOpts = new LoadOptions(LoadFormat.Html);
            
            // عيّن المنطقة إلى USA
            loadOpts.Region = CountryCode.USA;
            
            // تحميل ملف HTML مع إعدادات المنطقة المحددة
            Workbook wb = new Workbook("example.html", loadOpts);
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet ws = wb.Worksheets[0];
            
            // إظهار تنسيق مخصص للمنطقة عن طريق فحص نمط خلية
            Style style = ws.Cells["A1"].GetStyle();
            Console.WriteLine("Font used in cell A1: " + style.Font.Name);
            Console.WriteLine("Region used for loading: " + loadOpts.Region);
        }
    }
}
```

### انظر أيضًا

* enum [CountryCode](../../countrycode/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


