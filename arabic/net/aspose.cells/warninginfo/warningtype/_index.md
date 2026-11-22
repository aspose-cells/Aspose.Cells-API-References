---
title: "WarningInfo.WarningType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WarningInfo. الحصول على نوع التحذير"
type: docs
url: /ar/net/aspose.cells/warninginfo/warningtype/
---
## WarningInfo.WarningType property

احصل على نوع التحذير.

```csharp
[Obsolete("Use WarningInfo.Type property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public WarningType WarningType { get; }
```

### ملاحظات

ملاحظة: هذا العضو أصبح الآن غير صالح. بدلاً من ذلك، يرجى استخدام خاصية WarningInfo.Type. سيتم إزالة هذه الخاصية بعد 12 شهرًا اعتبارًا من ديسمبر 2024. تقدم Aspose اعتذارًا عن أي إزعاج قد تكون قد تعرضت له.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WarningInfoPropertyWarningTypeDemo
    {
        public static void Run()
        {
            // إنشاء مصنف وتفعيل التحذير
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // سيؤدي هذا إلى تفعيل تحذير عند الحفظ بميزات غير مدعومة
            workbook.Settings.WarningCallback = new WarningCallback();
            
            // احفظ بصيغة قد تتسبب في تحذيرات
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }

    internal class WarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            // عرض استخدام خاصية WarningType
            Console.WriteLine("Warning: " + warningInfo.WarningType + " - " + warningInfo.Description);
            
            // معالجة أنواع التحذير المحددة
            if (warningInfo.WarningType == WarningType.UnsupportedFileFormat)
            {
                Console.WriteLine("Unsupported format warning detected!");
            }
        }
    }
}
```

### انظر أيضًا

* enum [WarningType](../../warningtype/)
* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


