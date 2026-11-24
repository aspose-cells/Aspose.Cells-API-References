---
title: "WriteProtection.ValidatePassword"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WriteProtection-Methode. Gibt true zurück, wenn das angegebene Passwort mit dem Schreibschutz-Passwort übereinstimmt, mit dem die Datei geschützt wurde"
type: docs
url: /de/net/aspose.cells/writeprotection/validatepassword/
---
## WriteProtection.ValidatePassword method

Gibt true zurück, wenn das angegebene Passwort dem Schreibschutz‑Passwort entspricht, mit dem die Datei geschützt wurde.

```csharp
public bool ValidatePassword(string password)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Passwort | String | Das angegebene Passwort. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionMethodValidatePasswordWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Schreibschutz-Passwort festlegen
            workbook.Settings.WriteProtection.Password = "1234";
            
            // Passwort validieren
            Console.WriteLine("Password '1234' is valid: " + 
                workbook.Settings.WriteProtection.ValidatePassword("1234"));
            Console.WriteLine("Password 'wrong' is valid: " + 
                workbook.Settings.WriteProtection.ValidatePassword("wrong"));
        }
    }
}
```

### Siehe auch

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


