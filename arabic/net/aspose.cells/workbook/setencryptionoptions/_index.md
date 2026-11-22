---
title: "Workbook.SetEncryptionOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تعيين خيارات التشفير"
type: docs
url: /ar/net/aspose.cells/workbook/setencryptionoptions/
---
## Workbook.SetEncryptionOptions method

ضبط خيارات التشفير.

```csharp
public void SetEncryptionOptions(EncryptionType encryptionType, int keyLength)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| encryptionType | EncryptionType | نوع التشفير. |
| keyLength | Int32 | طول المفتاح. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSetEncryptionOptionsWithEncryptionTypeInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة بعض البيانات إلى ورقة العمل
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Encryption");
            
            // تعيين كلمة المرور وخيارات التشفير
            workbook.Settings.Password = "1234";
            workbook.SetEncryptionOptions(EncryptionType.StrongCryptographicProvider, 128);
            
            // حفظ دفتر العمل المشفر
            workbook.Save("EncryptedWorkbook.xls", SaveFormat.Excel97To2003);
            
            // التحقق بتحميل دفتر العمل المشفر
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.Password = "1234";
            Workbook encryptedWorkbook = new Workbook("EncryptedWorkbook.xls", loadOptions);
            
            Console.WriteLine("Workbook encrypted and loaded successfully.");
        }
    }
}
```

### انظر أيضًا

* enum [EncryptionType](../../encryptiontype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


