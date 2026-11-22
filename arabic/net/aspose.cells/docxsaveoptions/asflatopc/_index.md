---
title: "DocxSaveOptions.AsFlatOpc"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DocxSaveOptions. تشير إلى ما إذا كان الحفظ كملف flat opc يمكن إنشاؤه بواسطة Open XML SDK"
type: docs
url: /ar/net/aspose.cells/docxsaveoptions/asflatopc/
---
## DocxSaveOptions.AsFlatOpc property

يشير إلى ما إذا كان الحفظ كملف opc مسطح يمكن توليده بواسطة Open XML SDK

```csharp
public bool AsFlatOpc { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertyAsFlatOpcDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى وإضافة بيانات نموذجية
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Flat OPC Demo";

            try
            {
                // تهيئة DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // عرض القيمة الافتراضية لخاصية AsFlatOpc
                Console.WriteLine("Default AsFlatOpc value: " + saveOptions.AsFlatOpc);

                // تعيين AsFlatOpc إلى true لتوضيح استخدامها
                saveOptions.AsFlatOpc = true;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions.AsFlatOpc);

                // حفظ المصنف كملف DOCX باستخدام الخيارات المكوّنة
                workbook.Save("AsFlatOpcDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with AsFlatOpc option.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


