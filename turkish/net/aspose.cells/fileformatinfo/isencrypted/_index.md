---
title: "FileFormatInfo.IsEncrypted"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FileFormatInfo özelliği. Belge şifrelenmişse ve açmak için bir şifre gerektiriyorsa true döndürür"
type: docs
url: /tr/net/aspose.cells/fileformatinfo/isencrypted/
---
## FileFormatInfo.IsEncrypted property

Belge şifrelenmiş ve açmak için bir şifre gerektiriyorsa true döndürür.

```csharp
public bool IsEncrypted { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatInfoPropertyIsEncryptedDemo
    {
        public static void Run()
        {
            // Şifrelenmemiş bir dosyanın dosya biçimini tespit edin
            FileFormatInfo fileInfo = FileFormatUtil.DetectFileFormat("example.xlsx");
            Console.WriteLine("Is file encrypted? " + fileInfo.IsEncrypted);

            // Şifrelenmiş bir dosyanın dosya biçimini tespit edin
            FileFormatInfo encryptedFileInfo = FileFormatUtil.DetectFileFormat("encrypted.xlsx");
            Console.WriteLine("Is encrypted file encrypted? " + encryptedFileInfo.IsEncrypted);

            // Şifreli dosyayı şifreyle yükle
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Auto);
            loadOptions.Password = "password";
            Workbook workbook = new Workbook("encrypted.xlsx", loadOptions);
            Console.WriteLine("Encrypted file loaded successfully");
        }
    }
}
```

### Ayrıca Bakınız

* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


