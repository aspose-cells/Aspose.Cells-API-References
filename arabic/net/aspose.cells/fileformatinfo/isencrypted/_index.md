---
title: "FileFormatInfo.IsEncrypted"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FileFormatInfo. تُعيد true إذا كان المستند مشفرًا ويتطلب كلمة مرور للفتح"
type: docs
url: /ar/net/aspose.cells/fileformatinfo/isencrypted/
---
## FileFormatInfo.IsEncrypted property

يرجع true إذا كان المستند مشفرًا ويتطلب كلمة مرور للفتح.

```csharp
public bool IsEncrypted { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatInfoPropertyIsEncryptedDemo
    {
        public static void Run()
        {
            // اكتشف تنسيق ملف غير مشفر
            FileFormatInfo fileInfo = FileFormatUtil.DetectFileFormat("example.xlsx");
            Console.WriteLine("Is file encrypted? " + fileInfo.IsEncrypted);

            // اكتشف تنسيق ملف مشفر
            FileFormatInfo encryptedFileInfo = FileFormatUtil.DetectFileFormat("encrypted.xlsx");
            Console.WriteLine("Is encrypted file encrypted? " + encryptedFileInfo.IsEncrypted);

            // حمّل ملفًا مشفرًا باستخدام كلمة مرور
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Auto);
            loadOptions.Password = "password";
            Workbook workbook = new Workbook("encrypted.xlsx", loadOptions);
            Console.WriteLine("Encrypted file loaded successfully");
        }
    }
}
```

### انظر أيضًا

* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


