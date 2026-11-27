---
title: "WorkbookSettings.IsEncrypted"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings-egenskap. Hämtar ett värde som anger om ett lösenord krävs för att öppna denna arbetsbok"
type: docs
url: /sv/net/aspose.cells/workbooksettings/isencrypted/
---
## WorkbookSettings.IsEncrypted property

Hämtar ett värde som visar om ett lösenord krävs för att öppna denna arbetsbok.

```csharp
public bool IsEncrypted { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsEncryptedDemo
    {
        public static void Run()
        {
            // Exempel 1: Kontrollera om en lösenordsskyddad arbetsbok är krypterad
            string encryptedFilePath = "encrypted.xlsx";
            var encryptedWorkbook = new Workbook(encryptedFilePath, new LoadOptions { Password = "password" });
            Console.WriteLine($"Encrypted workbook IsEncrypted: {encryptedWorkbook.Settings.IsEncrypted}");

            // Exempel 2: Kontrollera om en normal arbetsbok är krypterad
            string normalFilePath = "normal.xlsx";
            var normalWorkbook = new Workbook(normalFilePath);
            Console.WriteLine($"Normal workbook IsEncrypted: {normalWorkbook.Settings.IsEncrypted}");

            // Exempel 3: Skapa och spara en krypterad arbetsbok
            var newWorkbook = new Workbook();
            newWorkbook.Settings.Password = "12345";
            newWorkbook.Save("new_encrypted.xlsx");
            Console.WriteLine($"New workbook IsEncrypted: {newWorkbook.Settings.IsEncrypted}");
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


