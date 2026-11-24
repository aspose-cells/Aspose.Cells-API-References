---
title: "Protection.AllowSelectingLockedCell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Schutz-Eigenschaft. Gibt an, ob der Benutzer gesperrte Zellen in einem geschützten Arbeitsblatt auswählen darf"
type: docs
url: /de/net/aspose.cells/protection/allowselectinglockedcell/
---
## Protection.AllowSelectingLockedCell property

Stellt dar, ob der Benutzer gesperrte Zellen in einem geschützten Arbeitsblatt auswählen darf.

```csharp
public bool AllowSelectingLockedCell { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowSelectingLockedCellDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Schutzeinstellungen festlegen
            Protection protection = worksheet.Protection;
            
            // Demonstriere die AllowSelectingLockedCell-Eigenschaft
            protection.AllowSelectingLockedCell = true;
            Console.WriteLine("AllowSelectingLockedCell is set to: " + protection.AllowSelectingLockedCell);

            // Ändere die Eigenschaft und zeige die Änderung
            protection.AllowSelectingLockedCell = false;
            Console.WriteLine("AllowSelectingLockedCell is now set to: " + protection.AllowSelectingLockedCell);

            // Schütze das Arbeitsblatt mit einem Passwort
            protection.Password = "password123";
            worksheet.Protect(ProtectionType.All);

            // Speichere die Arbeitsmappe
            workbook.Save("ProtectionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


