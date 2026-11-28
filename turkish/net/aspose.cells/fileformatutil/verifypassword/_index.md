---
title: "FileFormatUtil.VerifyPassword"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FileFormatUtil yöntemi. Bir akışta depolanan Excel'in formatı hakkında bilgiyi algılar ve döndürür"
type: docs
url: /tr/net/aspose.cells/fileformatutil/verifypassword/
---
## FileFormatUtil.VerifyPassword method

Bir akışta depolanan Excel'in formatı hakkında bilgiyi algılar ve döndürür.

```csharp
public static bool VerifyPassword(Stream stream, string password)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Stream |  |
| parola | String | Şifreli ooxml dosyaları için parola. |

### Dönüş Değeri

Parolanın doğru olup olmadığını döndürür.

### Örnekler

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

### Ayrıca Bakınız

* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


