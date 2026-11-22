---
title: "WorkbookSettings.Region"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. يحصل أو يضبط الإعدادات الإقليمية لدفتر العمل"
type: docs
url: /ar/net/aspose.cells/workbooksettings/region/
---
## WorkbookSettings.Region property

يحصل أو يضبط الإعدادات الإقليمية للمصنف.

```csharp
public CountryCode Region { get; set; }
```

### ملاحظات

1. الإعدادات الإقليمية التي يستخدمها مكوّن Aspose.Cells لدفتر عمل تم تحميله من ملف قالب: i). بالنسبة لملف XLS، هناك حقول معرفة للإعدادات الإقليمية وMS Excel يحفظ بيانات الإعدادات الإقليمية في الملف عند حفظ ملف XLS. لذلك، نستخدم المنطقة المحفوظة في ملف القالب لدفتر العمل. إذا لم ترغب في استخدام المنطقة المحفوظة في ملف XLS، يرجى إعادة تعيينها إلى القيمة المتوقعة (مثل CountryCode.Default) بعد تحميل ملف القالب. كما أننا نحفظ القيمة المحددة من قبل المستخدم (بهذه الطريقة) في الملف أيضًا عند حفظ ملف XLS. ii). بالنسبة لتنسيقات الملفات الأخرى، مثل XLSX، XLSB... إلخ، لا توجد حقل معرف للإعدادات الإقليمية في مواصفات تنسيق الملف. لذا نستخدم الإعدادات الإقليمية لبيئة التطبيق لدفتر العمل. ولا يمكن الاحتفاظ بالقيمة المحددة من قبل المستخدم (بهذه الطريقة) للملفات المُنشأة بتلك التنسيقات. 2. لتأثير العرض في MS Excel: الإعدادات الإقليمية المطبقة هنا يمكن أن تؤثر فقط أثناء وقت التشغيل مع مكوّن Aspose.Cells وليس عند عرض الملف المُنشأ باستخدام MS Excel. حتى بالنسبة لملف XLS المُنشأ الذي تم حفظ بيانات الإعدادات الإقليمية المحددة فيه، عند عرضه/تحريره باستخدام MS Excel، تكون المنطقة المستخدمة لتنسيق البيانات بواسطة MS Excel دائمًا هي الإعدادات الإقليمية الافتراضية للبيئة التي يعمل فيها MS Excel، وليس تلك المحفوظة في الملف. هذا سلوك MS Excel ولا يمكن تغييره عبر الشيفرة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyRegionDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.Japan;
            
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            cell.PutValue(44089); // Represents 2020-09-15
            
            Style style = cell.GetStyle();
            style.Custom = "[$-F800]yyyy年m月d日";
            cell.SetStyle(style);
            
            Console.WriteLine("Formatted value: " + cell.StringValue);
        }
    }
}
```

### انظر أيضًا

* enum [CountryCode](../../countrycode/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


