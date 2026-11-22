---
title: "WorkbookSettings.IsEncrypted"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تحصل على قيمة تشير إلى ما إذا كانت كلمة المرور مطلوبة لفتح هذا المصنف"
type: docs
url: /ar/net/aspose.cells/workbooksettings/isencrypted/
---
## WorkbookSettings.IsEncrypted property

يحصل على قيمة تشير إلى ما إذا كانت كلمة المرور مطلوبة لفتح هذا المصنف.

```csharp
public bool IsEncrypted { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsEncryptedDemo
    {
        public static void Run()
        {
            // المثال 1: التحقق مما إذا كان المصنف المحمي بكلمة مرور مشفرًا
            string encryptedFilePath = "encrypted.xlsx";
            var encryptedWorkbook = new Workbook(encryptedFilePath, new LoadOptions { Password = "password" });
            Console.WriteLine($"Encrypted workbook IsEncrypted: {encryptedWorkbook.Settings.IsEncrypted}");

            // المثال 2: التحقق مما إذا كان المصنف العادي مشفرًا
            string normalFilePath = "normal.xlsx";
            var normalWorkbook = new Workbook(normalFilePath);
            Console.WriteLine($"Normal workbook IsEncrypted: {normalWorkbook.Settings.IsEncrypted}");

            // المثال 3: إنشاء وحفظ مصنف مشفر
            var newWorkbook = new Workbook();
            newWorkbook.Settings.Password = "12345";
            newWorkbook.Save("new_encrypted.xlsx");
            Console.WriteLine($"New workbook IsEncrypted: {newWorkbook.Settings.IsEncrypted}");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


