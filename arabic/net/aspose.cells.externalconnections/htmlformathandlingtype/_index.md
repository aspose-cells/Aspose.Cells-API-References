---
title: "Enum HtmlFormatHandlingType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.ExternalConnections.HtmlFormatHandlingType enum. يحدد كيفية معالجة التنسيق من مصدر HTML"
type: docs
url: /ar/net/aspose.cells.externalconnections/htmlformathandlingtype/
---
## HtmlFormatHandlingType enumeration

يحدد كيفية التعامل مع التنسيق من مصدر HTML

```csharp
public enum HtmlFormatHandlingType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| All | `0` | نقل جميع تنسيقات HTML إلى ورقة العمل مع البيانات. |
| None | `1` | إدخال البيانات كنص غير منسق (لا يزال يتم تعيين أنواع البيانات). |
| Rtf | `2` | تحويل تنسيق HTML إلى تنسيق نص غني للبيانات التي تم إدخالها إلى ورقة العمل. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassHtmlFormatHandlingTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // عرض جميع قيم enum الخاصة بـ HtmlFormatHandlingType
                HtmlFormatHandlingType allFormatting = HtmlFormatHandlingType.All;
                HtmlFormatHandlingType noFormatting = HtmlFormatHandlingType.None;
                HtmlFormatHandlingType rtfFormatting = HtmlFormatHandlingType.Rtf;

                // عرض قيم التعداد
                Console.WriteLine("HtmlFormatHandlingType.All: " + allFormatting);
                Console.WriteLine("HtmlFormatHandlingType.None: " + noFormatting);
                Console.WriteLine("HtmlFormatHandlingType.Rtf: " + rtfFormatting);

                // محاكاة استخدام هذه القيم في سيناريو
                worksheet.Cells["A1"].PutValue("Format Handling Types:");
                worksheet.Cells["A2"].PutValue("All Formatting");
                worksheet.Cells["A3"].PutValue("No Formatting");
                worksheet.Cells["A4"].PutValue("RTF Formatting");

                // احفظ المصنف
                workbook.Save("HtmlFormatHandlingTypeDemo.xlsx");
                Console.WriteLine("Demo completed successfully. File saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in HtmlFormatHandlingType demo: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


