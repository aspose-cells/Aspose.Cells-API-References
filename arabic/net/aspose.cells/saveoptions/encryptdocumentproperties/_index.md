---
title: "SaveOptions.EncryptDocumentProperties"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SaveOptions. تشير إلى ما إذا كان سيتم تشفير خصائص المستند عند الحفظ كملف .xls. القيمة الافتراضية هي true"
type: docs
url: /ar/net/aspose.cells/saveoptions/encryptdocumentproperties/
---
## SaveOptions.EncryptDocumentProperties property

يشير إلى ما إذا كان سيتم تشفير خصائص المستند عند الحفظ كملف .xls. القيمة الافتراضية هي true.

```csharp
public bool EncryptDocumentProperties { get; set; }
```

### ملاحظات

فقط لملفات .xls, .xlsx, .xlsb و .xlsm.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyEncryptDocumentPropertiesDemo
    {
        public static void Run()
        {
            // إنشاء مصنف تجريبي
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // ضبط بعض خصائص المستند
            workbook.BuiltInDocumentProperties.Author = "Test Author";
            workbook.BuiltInDocumentProperties.Title = "Test Document";
            
            // تعيين حماية كلمة المرور
            workbook.Settings.Password = "password123";
            
            // حفظ مع EncryptDocumentProperties = true (الافتراضي)
            XlsSaveOptions saveOptions1 = new XlsSaveOptions();
            saveOptions1.EncryptDocumentProperties = true;
            workbook.Save("encrypted_properties.xls", saveOptions1);
            
            // حفظ مع EncryptDocumentProperties = false
            XlsSaveOptions saveOptions2 = new XlsSaveOptions();
            saveOptions2.EncryptDocumentProperties = false;
            workbook.Save("unencrypted_properties.xls", saveOptions2);
            
            // تحقق عن طريق إعادة التحميل
            Console.WriteLine("Files saved. Try opening them to see the difference in property encryption.");
        }
    }
}
```

### انظر أيضًا

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


