---
title: "WorkbookSettings.StreamProvider"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. يحصل على موفر التدفق للموارد الخارجية ويضبطه"
type: docs
url: /ar/net/aspose.cells/workbooksettings/streamprovider/
---
## WorkbookSettings.StreamProvider property

يحصل على موفر التدفق للموارد الخارجية ويضبطه.

```csharp
[Obsolete("Use ResourceProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IStreamProvider StreamProvider { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام خاصية ResourceProvider. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CustomStreamProvider1 : IStreamProvider
    {
        private MemoryStream stream;

        public void InitStream(StreamProviderOptions options)
        {
            stream = new MemoryStream();
            options.Stream = stream;
        }

        public void CloseStream(StreamProviderOptions options)
        {
            stream.Close();
            Console.WriteLine($"Stream closed. Content length: {stream.Length} bytes");
        }
    }

    public class WorkbookSettingsPropertyStreamProviderDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى إعدادات المصنف
            WorkbookSettings settings = workbook.Settings;

            // عرض قيمة StreamProvider الحالية
            Console.WriteLine("Current StreamProvider value: " + (settings.StreamProvider == null ? "null" : "custom provider"));

            // تعيين موفر تدفق مخصص
            settings.StreamProvider = new CustomStreamProvider1();

            // إضافة بعض البيانات لتوضيح استخدام التدفق
            worksheet.Cells["A1"].PutValue("Test data for stream provider");

            // حفظ المصنف - سيؤدي ذلك إلى تشغيل موفر التدفق
            workbook.Save("PropertyStreamProviderDemo.xlsx");

            // إعادة تعيين موفر التدفق
            settings.StreamProvider = null;
            Console.WriteLine("StreamProvider reset to null");
        }
    }
}
```

### انظر أيضًا

* interface [IStreamProvider](../../istreamprovider/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


