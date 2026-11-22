---
title: "Worksheet.Copy"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. تنسخ المحتويات والتنسيقات من ورقة عمل أخرى"
type: docs
url: /ar/net/aspose.cells/worksheet/copy/
---
## Copy(Worksheet) {#copy}

ينسخ المحتويات والتنسيقات من ورقة عمل أخرى.

```csharp
public void Copy(Worksheet sourceSheet)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceSheet | ورقة العمل | ورقة العمل المصدر. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCopyWithWorksheetDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل مصدر يحتوي على بيانات نموذجية
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Worksheet");
            
            // إنشاء دفتر عمل هدف
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // انسخ ورقة العمل المصدر إلى ورقة العمل الوجهة
            destSheet.Copy(sourceSheet);
            
            // حفظ النتيجة
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Copy(Worksheet, CopyOptions) {#copy_1}

ينسخ المحتويات والتنسيقات من ورقة عمل أخرى.

```csharp
public void Copy(Worksheet sourceSheet, CopyOptions copyOptions)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceSheet | ورقة العمل | ورقة العمل المصدر. |
| copyOptions | CopyOptions |  |

### ملاحظات

يمكنك نسخ البيانات من ورقة عمل أخرى في نفس الملف أو ملف آخر. ومع ذلك، لا تدعم هذه الطريقة نسخ كائنات الرسم، مثل التعليقات والصور والرسوم البيانية.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCopyWithWorksheetCopyOptionsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف المصدر مع بيانات عينة
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            srcSheet.Name = "SourceSheet";
            srcSheet.Cells["A1"].PutValue("Source Data");

            // إنشاء دفتر عمل هدف
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            destSheet.Name = "DestinationSheet";

            // تكوين خيارات النسخ
            CopyOptions options = new CopyOptions();
            options.ReferToDestinationSheet = true;

            // نسخ ورقة العمل مع الخيارات
            srcSheet.Copy(destSheet, options);

            // تحقق من عملية النسخ
            Console.WriteLine("Copied cell value: " + destSheet.Cells["A1"].StringValue);
            
            // حفظ النتيجة
            destWorkbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [CopyOptions](../../copyoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


