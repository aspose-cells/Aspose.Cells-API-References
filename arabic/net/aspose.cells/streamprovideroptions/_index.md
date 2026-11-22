---
title: "الفئة StreamProviderOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.StreamProviderOptions. تمثل خيارات الدفق"
type: docs
url: /ar/net/aspose.cells/streamprovideroptions/
---
## StreamProviderOptions class

يمثل خيارات الدفق.

```csharp
public class StreamProviderOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [StreamProviderOptions](streamprovideroptions/#constructor)() | تهيئة نسخة جديدة من الفئة `StreamProviderOptions`. |
| [StreamProviderOptions](streamprovideroptions/#constructor_1)(ResourceLoadingType, string) | تهيئة نسخة جديدة من الفئة `StreamProviderOptions`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CustomPath](../../aspose.cells/streamprovideroptions/custompath/) { get; set; } | المسار المخصص (URL) للمستخدم المحفوظ في ملف HTML المُولد للمصدر المشار إليه. إذا لم يحدده المستخدم، سيتم استخدام DefaultPath. على سبيل المثال، سيتم حفظ بيانات الورقة من قبل المستخدم إلى d:/sheet001.htm، ويجب أن يكون عنوان URL المستخدم في ملف HTML الرئيسي هو "d:/sheet001.htm" أو أي مسار نسبي صالح آخر يمكن الوصول إليه من ملف HTML الرئيسي. |
| [DefaultPath](../../aspose.cells/streamprovideroptions/defaultpath/) { get; } | المسار الافتراضي (URL) المحفوظ في ملف html المُولد للمصدر المشار إليه. على سبيل المثال، يتم حفظ بيانات الورقة في xxx_files/sheet001.htm، يجب أن يكون عنوان url المستخدم في ملف html الرئيسي مثل "src=\"xxx_files/sheet001.htm\"" |
| [ResourceLoadingType](../../aspose.cells/streamprovideroptions/resourceloadingtype/) { get; set; } | يحصل ويضبط نوع مورد التحميل. |
| [Stream](../../aspose.cells/streamprovideroptions/stream/) { get; set; } | يحصل/يضبط الدفق |

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassStreamProviderOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إنشاء StreamProviderOptions
            StreamProviderOptions options = new StreamProviderOptions();
            
            // تعيين دفق ذاكرة للعرض
            options.Stream = new MemoryStream();
            
            // استخدام الدفق (مثال: حفظ المصنف إلى الدفق)
            workbook.Save(options.Stream, SaveFormat.Xlsx);
            
            // إظهار إغلاق الدفق
            CloseStream(options);
        }

        public static void CloseStream(StreamProviderOptions options)
        {
            if (options.Stream != null)
            {
                options.Stream.Close();
                options.Stream = null;
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


