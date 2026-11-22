---
title: "PclSaveOptions.PclSaveOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ PclSaveOptions. ينشئ الخيارات لحفظ ملف pcl"
type: docs
url: /ar/net/aspose.cells/pclsaveoptions/pclsaveoptions/
---
## PclSaveOptions constructor

ينشئ الخيارات لحفظ ملف pcl.

```csharp
public PclSaveOptions()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PclSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بعض البيانات النموذجية إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("PCL Save Options Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates PclSaveOptions constructor");
            
            try
            {
                // استدعِ طريقة #ctor لإنشاء مثيل PclSaveOptions
                PclSaveOptions pclOptions = new PclSaveOptions();
                
                // قم بتكوين الخيارات الإضافية إذا لزم الأمر
                pclOptions.AddPrinterFont("Arial", "ArialPCL");
                
                Console.WriteLine("PclSaveOptions created successfully");
                
                // احفظ المصنف باستخدام خيارات PCL.
                workbook.Save("PclSaveOptionsDemo.pcl", pclOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating PclSaveOptions: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


