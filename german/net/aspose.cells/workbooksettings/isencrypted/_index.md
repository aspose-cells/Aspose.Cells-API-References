---
title: "WorkbookSettings.IsEncrypted"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt einen Wert zurück, der angibt, ob ein Passwort zum Öffnen dieser Arbeitsmappe erforderlich ist"
type: docs
url: /de/net/aspose.cells/workbooksettings/isencrypted/
---
## WorkbookSettings.IsEncrypted property

Liest einen Wert, der angibt, ob für das Öffnen dieses Workbooks ein Passwort erforderlich ist.

```csharp
public bool IsEncrypted { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsEncryptedDemo
    {
        public static void Run()
        {
            // Beispiel 1: Prüfen, ob eine passwortgeschützte Arbeitsmappe verschlüsselt ist
            string encryptedFilePath = "encrypted.xlsx";
            var encryptedWorkbook = new Workbook(encryptedFilePath, new LoadOptions { Password = "password" });
            Console.WriteLine($"Encrypted workbook IsEncrypted: {encryptedWorkbook.Settings.IsEncrypted}");

            // Beispiel 2: Prüfen, ob eine normale Arbeitsmappe verschlüsselt ist
            string normalFilePath = "normal.xlsx";
            var normalWorkbook = new Workbook(normalFilePath);
            Console.WriteLine($"Normal workbook IsEncrypted: {normalWorkbook.Settings.IsEncrypted}");

            // Beispiel 3: Eine verschlüsselte Arbeitsmappe erstellen und speichern
            var newWorkbook = new Workbook();
            newWorkbook.Settings.Password = "12345";
            newWorkbook.Save("new_encrypted.xlsx");
            Console.WriteLine($"New workbook IsEncrypted: {newWorkbook.Settings.IsEncrypted}");
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


