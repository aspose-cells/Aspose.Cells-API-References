---
title: "FileFormatInfo.IsEncrypted"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FileFormatInfo Eigenschaft. Gibt true zurück, wenn das Dokument verschlüsselt ist und ein Passwort zum Öffnen benötigt"
type: docs
url: /de/net/aspose.cells/fileformatinfo/isencrypted/
---
## FileFormatInfo.IsEncrypted property

Gibt true zurück, wenn das Dokument verschlüsselt ist und ein Passwort zum Öffnen benötigt.

```csharp
public bool IsEncrypted { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatInfoPropertyIsEncryptedDemo
    {
        public static void Run()
        {
            // Dateiformat einer nicht verschlüsselten Datei erkennen
            FileFormatInfo fileInfo = FileFormatUtil.DetectFileFormat("example.xlsx");
            Console.WriteLine("Is file encrypted? " + fileInfo.IsEncrypted);

            // Dateiformat einer verschlüsselten Datei erkennen
            FileFormatInfo encryptedFileInfo = FileFormatUtil.DetectFileFormat("encrypted.xlsx");
            Console.WriteLine("Is encrypted file encrypted? " + encryptedFileInfo.IsEncrypted);

            // Verschlüsselte Datei mit Passwort laden
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Auto);
            loadOptions.Password = "password";
            Workbook workbook = new Workbook("encrypted.xlsx", loadOptions);
            Console.WriteLine("Encrypted file loaded successfully");
        }
    }
}
```

### Siehe auch

* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


