---
title: "IExportObjectListener.ExportObject"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة IExportObjectListener. صدّر كائنًا واحدًا"
type: docs
url: /ar/net/aspose.cells/iexportobjectlistener/exportobject/
---
## IExportObjectListener.ExportObject method

صدّر كائنًا واحدًا.

```csharp
public object ExportObject(ExportObjectEvent e)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| e | ExportObjectEvent | الحدث الذي يتم تشغيله عندما يحتاج كائن واحد إلى التصدير. |

### قيمة الإرجاع

المعلومات حول نتيجة تصدير الكائن. عند تصدير الكائنات عند تصدير المصنف إلى تنسيق HTML، تكون النتيجة سلسلة URL للوصول إلى الصورة المحفوظة من ملف HTML الذي يحتوي على هذا الكائن المصدر.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class IExportObjectListenerMethodExportObjectWithExportObjectEventDemo : IExportObjectListener
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف صورة إلى ورقة العمل
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // أنشئ مثيلًا لفئة العرض التوضيحي التي تنفّذ IExportObjectListener
            var listener = new IExportObjectListenerMethodExportObjectWithExportObjectEventDemo();

            try
            {
                // في سيناريو حقيقي، سيتم توفير ExportObjectEvent من قبل الإطار
                // لأغراض العرض التوضيحي، سنستدعي الطريقة فقط مع null
                object result = listener.ExportObject(null);

                Console.WriteLine("ExportObject method executed successfully.");
                Console.WriteLine($"Returned object type: {result?.GetType().Name ?? "null"}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ExportObject method: {ex.Message}");
            }

            workbook.Save("ExportObjectDemo.xlsx");
        }

        public object ExportObject(ExportObjectEvent e)
        {
            // تنفيذ مخصص لمعالجة التصدير
            if (e != null)
            {
                object source = e.GetSource();
                Console.WriteLine($"Exporting object of type: {source?.GetType().Name ?? "null"}");
            }
            else
            {
                Console.WriteLine("No export event provided (demo mode)");
            }

            // أرجع كائنًا معدلًا أو null لاستخدام سلوك التصدير الافتراضي
            return null;
        }
    }
}
```

### انظر أيضًا

* class [ExportObjectEvent](../../exportobjectevent/)
* interface [IExportObjectListener](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


