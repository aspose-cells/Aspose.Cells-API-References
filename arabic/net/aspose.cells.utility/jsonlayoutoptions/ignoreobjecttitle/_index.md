---
title: "JsonLayoutOptions.IgnoreObjectTitle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية JsonLayoutOptions. تشير إلى ما إذا كان يتم تجاهل العنوان إذا كان الكائن خاصية لكائن"
type: docs
url: /ar/net/aspose.cells.utility/jsonlayoutoptions/ignoreobjecttitle/
---
## JsonLayoutOptions.IgnoreObjectTitle property

تشير إلى ما إذا كان يتم تجاهل العنوان إذا كان الكائن خاصية لكائن.

```csharp
[Obsolete("Use JsonLayoutOptions.IgnoreTitle property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IgnoreObjectTitle { get; set; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية JsonLayoutOptions.IgnoreTitle. سيتم إزالة هذه الخاصية بعد 6 أشهر منذ فبراير 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class JsonLayoutOptionsPropertyIgnoreObjectTitleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // بيانات JSON نموذجية مع عناوين الكائنات
            string json = @"{
                ""Employees"": {
                    ""Employee"": [
                        { ""Name"": ""John"", ""Age"": 30 },
                        { ""Name"": ""Jane"", ""Age"": 25 }
                    ]
                }
            }";

            // إنشاء JsonLayoutOptions
            JsonLayoutOptions options = new JsonLayoutOptions();
            
            // عرض قيمة IgnoreObjectTitle الحالية
            Console.WriteLine("Current IgnoreObjectTitle value: " + options.IgnoreObjectTitle);

            // تعيين لتجاهل عناوين الكائنات
            options.IgnoreObjectTitle = true;
            Console.WriteLine("Set IgnoreObjectTitle to: " + options.IgnoreObjectTitle);

            // استيراد JSON مع IgnoreObjectTitle = true
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);

            // حفظ مع العناوين المتجاهلة
            workbook.Save("IgnoreObjectTitle_True.xlsx");

            // إعادة تعيين ورقة العمل
            worksheet.Cells.Clear();

            // تعيين لتضمين عناوين الكائنات
            options.IgnoreObjectTitle = false;
            Console.WriteLine("Set IgnoreObjectTitle to: " + options.IgnoreObjectTitle);

            // استيراد JSON مع IgnoreObjectTitle = false
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);

            // حفظ مع العناوين المتضمنة
            workbook.Save("IgnoreObjectTitle_False.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


