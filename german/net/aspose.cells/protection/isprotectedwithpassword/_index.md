---
title: "Protection.IsProtectedWithPassword"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Protection-Eigenschaft. Gibt an, ob das Arbeitsblatt mit einem Passwort geschützt ist."
type: docs
url: /de/net/aspose.cells/protection/isprotectedwithpassword/
---
## Protection.IsProtectedWithPassword property

Gibt an, ob das Arbeitsblatt mit einem Passwort geschützt ist.

```csharp
public bool IsProtectedWithPassword { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyIsProtectedWithPasswordDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Auf die Schutzeinstellungen des Arbeitsblatts zugreifen
            Protection protection = worksheet.Protection;

            // Schutz-Passwort festlegen
            protection.Password = "test123";

            // Überprüfen, ob das Arbeitsblatt passwortgeschützt ist
            bool isProtectedWithPassword = protection.IsProtectedWithPassword;
            Console.WriteLine("Is worksheet protected with password: " + isProtectedWithPassword);

            // Speichere die Arbeitsmappe
            workbook.Save("PasswordProtectionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


