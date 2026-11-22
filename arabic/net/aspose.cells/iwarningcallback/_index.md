---
title: "الواجهة IWarningCallback"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "واجهة Aspose.Cells.IWarningCallback. واجهة رد الاتصال للتحذير"
type: docs
url: /ar/net/aspose.cells/iwarningcallback/
---
## IWarningCallback interface

واجهة الاستدعاء للتحذير.

```csharp
public interface IWarningCallback
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Warning](../../aspose.cells/iwarningcallback/warning/)(WarningInfo) | يحتاج رد الاتصال الخاص بنا فقط إلى تنفيذ طريقة "Warning". |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IWarningCallbackDemo : IWarningCallback
    {
        // تنفيذ طريقة Warning من واجهة IWarningCallback
        public void Warning(WarningInfo warningInfo)
        {
            // عرض رسالة التحذير
            Console.WriteLine("Warning: " + warningInfo.WarningType + " - " + warningInfo.Description);
        }

        public static void IWarningCallbackExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // تعيين رد الاتصال للتحذير
            workbook.Settings.WarningCallback = new IWarningCallbackDemo();

            // تحميل دفتر عمل مع تحذيرات محتملة
            try
            {
                workbook = new Workbook("example.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Exception: " + ex.Message);
            }

            // احفظ المصنف
            workbook.Save("IWarningCallbackExample.xlsx");
        }
    }

}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


