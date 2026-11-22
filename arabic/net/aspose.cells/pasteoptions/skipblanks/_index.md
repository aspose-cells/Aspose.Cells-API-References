---
title: "PasteOptions.SkipBlanks"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PasteOptions. تشير إلى ما إذا كان يتخطى الخلايا الفارغة"
type: docs
url: /ar/net/aspose.cells/pasteoptions/skipblanks/
---
## PasteOptions.SkipBlanks property

يشير إلى ما إذا كان يتخطى الخلايا الفارغة.

```csharp
public bool SkipBlanks { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertySkipBlanksDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل مصدر يحتوي على بيانات نموذجية
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // ملء النطاق المصدر ببعض القيم والفارغات
            sourceSheet.Cells["A1"].PutValue("Value 1");
            sourceSheet.Cells["A2"].PutValue(""); // Blank cell
            sourceSheet.Cells["A3"].PutValue("Value 3");
            sourceSheet.Cells["A4"].PutValue(""); // Blank cell
            
            // إنشاء دفتر عمل هدف
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // ملء النطاق الوجهة بالقيم الموجودة
            destSheet.Cells["A1"].PutValue("Existing 1");
            destSheet.Cells["A2"].PutValue("Existing 2");
            destSheet.Cells["A3"].PutValue("Existing 3");
            destSheet.Cells["A4"].PutValue("Existing 4");
            
            // الحصول على النطاقات بأسماء الأنواع المؤهلة بالكامل
            Aspose.Cells.Range sourceRange = sourceSheet.Cells.CreateRange("A1:A4");
            Aspose.Cells.Range destRange = destSheet.Cells.CreateRange("A1:A4");
            
            // نسخ مع SkipBlanks = true (الافتراضي)
            destRange.Copy(sourceRange, new PasteOptions { SkipBlanks = true });
            
            Console.WriteLine("Results with SkipBlanks=true:");
            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {destSheet.Cells[i, 0].StringValue}");
            }
            
            // إعادة تعيين قيم الوجهة
            destSheet.Cells["A1"].PutValue("Existing 1");
            destSheet.Cells["A2"].PutValue("Existing 2");
            destSheet.Cells["A3"].PutValue("Existing 3");
            destSheet.Cells["A4"].PutValue("Existing 4");
            
            // نسخ مع SkipBlanks = false
            destRange.Copy(sourceRange, new PasteOptions { SkipBlanks = false });
            
            Console.WriteLine("\nResults with SkipBlanks=false:");
            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {destSheet.Cells[i, 0].StringValue}");
            }
        }
    }
}
```

### انظر أيضًا

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


