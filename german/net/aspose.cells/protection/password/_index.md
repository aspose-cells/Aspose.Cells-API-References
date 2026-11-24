---
title: "Protection.Password"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Protection-Eigenschaft. Gibt das Passwort zum Schutz des Arbeitsblatts an."
type: docs
url: /de/net/aspose.cells/protection/password/
---
## Protection.Password property

Stellt das Passwort zum Schutz des Arbeitsblatts dar.

```csharp
public string Password { get; set; }
```

### Hinweise

Wenn das Passwort auf null oder einen leeren String gesetzt ist, können Sie das Arbeitsblatt oder die Arbeitsmappe ohne Passwort entsperren. Andernfalls müssen Sie das Passwort angeben, um das Arbeitsblatt oder die Arbeitsmappe zu entsperren.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyPasswordDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Schutzeinstellungen mit Passwort festlegen
            Protection protection = worksheet.Protection;
            protection.AllowEditingContent = false;
            protection.AllowDeletingColumn = false;
            protection.Password = "test123";

            // Verifiziere den Passwortschutz
            Console.WriteLine("Worksheet is protected: " + (protection.Password != null));
            Console.WriteLine("Protection password: " + protection.Password);

            // Erstelle ein weiteres Protection-Objekt zum Vergleich
            Protection protection2 = worksheet.Protection;
            protection2.Password = "test123";

            // Vergleiche den Passwortschutz
            Console.WriteLine("Passwords match: " + (protection.Password == protection2.Password));
        }
    }
}
```

### Siehe auch

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


