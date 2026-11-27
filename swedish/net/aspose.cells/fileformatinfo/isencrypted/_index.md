---
title: "FileFormatInfo.IsEncrypted"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FileFormatInfo-egenskap. Returnerar true om dokumentet är krypterat och kräver ett lösenord för att öppna"
type: docs
url: /sv/net/aspose.cells/fileformatinfo/isencrypted/
---
## FileFormatInfo.IsEncrypted property

Returnerar true om dokumentet är krypterat och kräver ett lösenord för att öppnas.

```csharp
public bool IsEncrypted { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatInfoPropertyIsEncryptedDemo
    {
        public static void Run()
        {
            // Detektera filformat för en okrypterad fil
            FileFormatInfo fileInfo = FileFormatUtil.DetectFileFormat("example.xlsx");
            Console.WriteLine("Is file encrypted? " + fileInfo.IsEncrypted);

            // Detektera filformat för en krypterad fil
            FileFormatInfo encryptedFileInfo = FileFormatUtil.DetectFileFormat("encrypted.xlsx");
            Console.WriteLine("Is encrypted file encrypted? " + encryptedFileInfo.IsEncrypted);

            // Läs in krypterad fil med lösenord
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Auto);
            loadOptions.Password = "password";
            Workbook workbook = new Workbook("encrypted.xlsx", loadOptions);
            Console.WriteLine("Encrypted file loaded successfully");
        }
    }
}
```

### Se även

* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


