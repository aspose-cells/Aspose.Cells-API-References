---
title: "VbaProject.ValidatePassword"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaProject-Methode. Validiert das Schutzpasswort"
type: docs
url: /de/net/aspose.cells.vba/vbaproject/validatepassword/
---
## VbaProject.ValidatePassword method

Validiert das Schutzkennwort.

```csharp
public bool ValidatePassword(string password)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Passwort | String | das Passwort |

### Rückgabewert

Ob das Passwort das Schutzpasswort dieses VBA-Projekts ist

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectMethodValidatePasswordWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein Arbeitsbuchobjekt aus einer Beispiel‑Excel‑Datei mit VBA‑Projekt
            Workbook workbook = new Workbook("example.xlsm");
            
            // Validiere das VBA-Projektpasswort
            bool isValid = workbook.VbaProject.ValidatePassword("test");
            
            // Gib das Validierungsergebnis aus
            Console.WriteLine("Password validation result: " + isValid);
        }
    }
}
```

### Siehe auch

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


