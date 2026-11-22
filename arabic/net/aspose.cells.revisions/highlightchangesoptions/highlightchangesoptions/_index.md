---
title: "HighlightChangesOptions.HighlightChangesOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ HighlightChangesOptions. يمثل خيارات تمييز المراجعات أو التغييرات في ملفات Excel المشتركة"
type: docs
url: /ar/net/aspose.cells.revisions/highlightchangesoptions/highlightchangesoptions/
---
## HighlightChangesOptions constructor

يمثل خيارات تمييز المراجعات أو التغييرات في ملفات إكسل المشتركة.

```csharp
public HighlightChangesOptions(bool highlightOnScreen, bool listOnNewSheet)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| highlightOnScreen | منطقي | يشير إلى ما إذا كان يتم تمييز التغييرات على الشاشة. |
| listOnNewSheet | منطقي | يشير إلى ما إذا كان يتم سرد التغييرات في ورقة عمل جديدة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class HighlightChangesOptionsMethodCtorWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف بعض البيانات التجريبية
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Original Value");
            worksheet.Cells["A2"].PutValue(100);
            
            // إنشاء HighlightChangesOptions باستخدام معلمات منطقية
            HighlightChangesOptions options = new HighlightChangesOptions(true, true);
            
            // محاكاة تتبع التغييرات (عادةً ما تكون لديك مراجعات فعلية)
            Console.WriteLine("HighlightChangesOptions created with:");
            Console.WriteLine($"First parameter (show changes): {true}");
            Console.WriteLine($"Second parameter (changes on new sheet): {true}");
            
            // احفظ المصنف
            workbook.Save("HighlightChangesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HighlightChangesOptions](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


