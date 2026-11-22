---
title: "Workbook.AcceptAllRevisions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تقبل جميع التغييرات المتتبعة في المصنف"
type: docs
url: /ar/net/aspose.cells/workbook/acceptallrevisions/
---
## Workbook.AcceptAllRevisions method

يقبل جميع التغييرات المتتبعة في المصنف.

```csharp
public void AcceptAllRevisions()
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodAcceptAllRevisionsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف مع مراجعات
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بعض المراجعات (يجب تمكين تتبع التغييرات في Excel أولاً)
            worksheet.Cells["A1"].PutValue("Original Value");
            
            // احفظ مع المراجعات
            string sourcePath = "source_with_revisions.xlsx";
            workbook.Save(sourcePath, SaveFormat.Xlsx);
            
            // أعد فتح المصنف
            workbook = new Workbook(sourcePath);
            
            // تحقق مما إذا كان يحتوي على مراجعات وقم بقبولها
            if (workbook.HasRevisions)
            {
                Console.WriteLine("Workbook has revisions. Accepting all...");
                workbook.AcceptAllRevisions();
                
                // احفظ بدون مراجعات
                string destPath = "output_no_revisions.xlsx";
                workbook.Save(destPath, SaveFormat.Xlsx);
                Console.WriteLine("Revisions accepted and saved to: " + destPath);
            }
            else
            {
                Console.WriteLine("Workbook has no revisions.");
            }
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


