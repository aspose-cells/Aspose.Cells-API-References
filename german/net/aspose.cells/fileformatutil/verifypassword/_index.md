---
title: "FileFormatUtil.VerifyPassword"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FileFormatUtil-Methode. Erkennt und gibt die Informationen über ein Excel-Format zurück, das in einem Stream gespeichert ist"
type: docs
url: /de/net/aspose.cells/fileformatutil/verifypassword/
---
## FileFormatUtil.VerifyPassword method

Erkennt und gibt die Informationen über das Format einer in einem Stream gespeicherten Excel-Datei zurück.

```csharp
public static bool VerifyPassword(Stream stream, string password)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | Stream |  |
| Passwort | String | Das Passwort für verschlüsselte ooxml-Dateien. |

### Rückgabewert

Gibt zurück, ob das Passwort korrekt ist.

### Beispiele

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

### Siehe auch

* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


