---
title: "CopyOptions.CopyNames"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CopyOptions. تشير إلى ما إذا كان يتم نسخ الأسماء"
type: docs
url: /ar/net/aspose.cells/copyoptions/copynames/
---
## CopyOptions.CopyNames property

يشير إلى ما إذا كان يتم نسخ الأسماء.

```csharp
public bool CopyNames { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyCopyNamesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل مصدر يحتوي على نطاقات مسماة
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // إنشاء نطاق مسمى في دفتر العمل المصدر
            sourceSheet.Cells["A1"].PutValue("Test Value");
            int index = sourceWorkbook.Worksheets.Names.Add("SourceName");
            sourceWorkbook.Worksheets.Names[index].RefersTo = "=Sheet1!$A$1";

            // إنشاء دفتر عمل هدف
            Workbook destWorkbook = new Workbook();
            
            // نسخ ورقة العمل مع CopyNames=true
            destWorkbook.Worksheets[0].Copy(sourceSheet, new CopyOptions { CopyNames = true });

            // تحقق من أنه تم نسخ النطاق المسمى
            Name copiedName = destWorkbook.Worksheets.Names["SourceName"];
            if (copiedName != null)
            {
                Console.WriteLine("Named range copied successfully: " + copiedName.RefersTo);
            }
            else
            {
                Console.WriteLine("Named range was not copied");
            }
        }
    }
}
```

### انظر أيضًا

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


