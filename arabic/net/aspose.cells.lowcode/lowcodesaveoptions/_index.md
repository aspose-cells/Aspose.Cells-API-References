---
title: "فئة LowCodeSaveOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.LowCode.LowCodeSaveOptions. خيارات حفظ النتائج المُولدة بطريقة منخفضة الكود"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodesaveoptions/
---
## LowCodeSaveOptions class

خيارات حفظ النتائج المولدة بطريقة منخفضة الكود.

```csharp
public class LowCodeSaveOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [LowCodeSaveOptions](lowcodesaveoptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | الحصول وتعيين الملف (مع المسار إذا لزم) لحفظ البيانات المُولدة. عند تعيين هذه الخاصية بقيمة غير null أو سلسلة فارغة، سيتم تجاهل [`OutputStream`](./outputstream/). |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | الحصول وتعيين الدفق لكتابة البيانات المُولدة إليه. عند تعيين هذه الخاصية بقيمة غير null، سيتم تجاهل [`OutputFile`](./outputfile/). |
| virtual [SaveFormat](../../aspose.cells.lowcode/lowcodesaveoptions/saveformat/) { get; set; } | الحصول وتعيين تنسيق الحفظ للإخراج. عادةً، في عمليات محددة بطريقة منخفضة الكود، يُسمح فقط ببعض الصيغ المحددة. يرجى تحديد الصيغة الصحيحة للعملية المقابلة، وإلا قد يحدث نتيجة غير متوقعة أو حتى استثناء. |

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassLowCodeSaveOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف ورقة عمل وضع بعض البيانات
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // إنشاء خيارات الحفظ
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions()
            {
                OutputFile = "output.xlsx"
            };

            // احفظ المصنف باستخدام الخيارات المحددة
            workbook.Save(saveOptions.OutputFile, saveOptions.SaveFormat);
            
            Console.WriteLine("File saved successfully with LowCodeSaveOptions");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


