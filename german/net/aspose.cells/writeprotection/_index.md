---
title: "Klasse WriteProtection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.WriteProtection‑Klasse. Gibt die Schreibschutz‑Einstellungen für eine Arbeitsmappe an."
type: docs
url: /de/net/aspose.cells/writeprotection/
---
## WriteProtection class

Gibt die Schreibschutz‑Einstellungen für eine Arbeitsmappe an.

```csharp
public class WriteProtection
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Author](../../aspose.cells/writeprotection/author/) { get; set; } | Liest und setzt den Autor. |
| [IsWriteProtected](../../aspose.cells/writeprotection/iswriteprotected/) { get; } | Gibt an, ob diese Arbeitsmappe schreibgeschützt ist. |
| [Password](../../aspose.cells/writeprotection/password/) { get; set; } | Setzt das geschützte Passwort, um die Datei zu ändern. |
| [RecommendReadOnly](../../aspose.cells/writeprotection/recommendreadonly/) { get; set; } | Gibt an, ob die Option „Read Only Recommended“ ausgewählt ist. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [ValidatePassword](../../aspose.cells/writeprotection/validatepassword/)(string) | Gibt true zurück, wenn das angegebene Passwort dem Schreibschutz‑Passwort entspricht, mit dem die Datei geschützt wurde. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WriteProtectionDemo
    {
        public static void WriteProtectionExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Zugriff auf die Einstellungen der Arbeitsmappe
            WorkbookSettings settings = workbook.Settings;

            // Zugriff auf die Einstellungen des Schreibschutzes
            WriteProtection writeProtection = settings.WriteProtection;

            // Den Autor des Schreibschutzes festlegen
            writeProtection.Author = "John Doe";

            // Das Passwort für den Schreibschutz festlegen
            writeProtection.Password = "password123";

            // Die empfohlene Nur-Lese-Option festlegen
            writeProtection.RecommendReadOnly = true;

            // Prüfen, ob die Arbeitsmappe schreibgeschützt ist
            bool isWriteProtected = writeProtection.IsWriteProtected;
            Console.WriteLine("Is Write Protected: " + isWriteProtected);

            // Das Passwort validieren
            bool isValidPassword = writeProtection.ValidatePassword("password123");
            Console.WriteLine("Is Valid Password: " + isValidPassword);

            // Speichere die Arbeitsmappe
            workbook.Save("WriteProtectionExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


