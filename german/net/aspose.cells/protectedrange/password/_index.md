---
title: "ProtectedRange.Password"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ProtectedRange-Eigenschaft. Stellt das Passwort dar, um den Bereich zu schützen"
type: docs
url: /de/net/aspose.cells/protectedrange/password/
---
## ProtectedRange.Password property

Stellt das Passwort dar, um den Bereich zu schützen.

```csharp
public string Password { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertyPasswordDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Sammlung geschützter Bereiche
            ProtectedRangeCollection allowRanges = worksheet.AllowEditRanges;

            // Füge einen geschützten Bereich hinzu
            int index = allowRanges.Add("MyProtectedRange", 0, 0, 2, 2);
            ProtectedRange protectedRange = allowRanges[index];

            // Setze das Passwort für den geschützten Bereich
            protectedRange.Password = "12345";

            // Speichere die Arbeitsmappe
            workbook.Save("ProtectedRangeWithPassword.xlsx");
        }
    }
}
```

### Siehe auch

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


