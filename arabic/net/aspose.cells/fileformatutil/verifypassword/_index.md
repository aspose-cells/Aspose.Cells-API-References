---
title: "FileFormatUtil.VerifyPassword"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FileFormatUtil. يكتشف ويعيد المعلومات حول تنسيق ملف Excel المخزن في تدفق"
type: docs
url: /ar/net/aspose.cells/fileformatutil/verifypassword/
---
## FileFormatUtil.VerifyPassword method

يكشف ويعيد المعلومات حول تنسيق ملف إكسل المخزن في تدفق.

```csharp
public static bool VerifyPassword(Stream stream, string password)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | Stream |  |
| كلمة المرور | String | كلمة المرور للملفات ooxml المشفرة. |

### قيمة الإرجاع

يرجع ما إذا كانت كلمة المرور صحيحة.

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodVerifyPasswordWithStreamStringDemo
    {
        public static void Run()
        {
            string filePath = "example.xlsx";
            string correctPassword = "test";
            string wrongPassword = "1234";

            using (Stream stream = File.OpenRead(filePath))
            {
                bool isValid = FileFormatUtil.VerifyPassword(stream, correctPassword);
                Console.WriteLine($"Password '{correctPassword}' is valid: {isValid}");
            }

            using (Stream stream = File.OpenRead(filePath))
            {
                bool isValid = FileFormatUtil.VerifyPassword(stream, wrongPassword);
                Console.WriteLine($"Password '{wrongPassword}' is valid: {isValid}");
            }
        }
    }
}
```

### انظر أيضًا

* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


