---
title: "Protection.Copy"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Protection. نسخ معلومات الحماية"
type: docs
url: /ar/net/aspose.cells/protection/copy/
---
## Protection.Copy method

نسخ معلومات الحماية.

```csharp
public void Copy(Protection source)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المصدر | Protection |  |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectionMethodCopyWithProtectionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء إعدادات حماية المصدر - استخدم الحماية الحالية من ورقة العمل
            Protection sourceProtection = worksheet.Protection;
            sourceProtection.AllowDeletingColumn = true;
            sourceProtection.AllowInsertingRow = false;
            sourceProtection.Password = "test123";
            sourceProtection.AllowFormattingCell = true;

            // احصل على إعدادات الحماية المستهدفة
            Protection targetProtection = worksheet.Protection;

            try
            {
                // استدعِ طريقة Copy مع معامل Protection
                targetProtection.Copy(sourceProtection);

                Console.WriteLine("Protection settings copied successfully.");
                Console.WriteLine($"Target protection - AllowDeletingColumn: {targetProtection.AllowDeletingColumn}");
                Console.WriteLine($"Target protection - AllowInsertingRow: {targetProtection.AllowInsertingRow}");
                Console.WriteLine($"Target protection - Password set: {!string.IsNullOrEmpty(targetProtection.Password)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error copying protection settings: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("ProtectionCopyDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


