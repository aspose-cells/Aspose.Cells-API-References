---
title: "Protection.AllowSelectingUnlockedCell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Protection property. Gibt an, ob der Benutzer nicht gesperrte Zellen in einem geschützten Arbeitsblatt auswählen darf"
type: docs
url: /de/net/aspose.cells/protection/allowselectingunlockedcell/
---
## Protection.AllowSelectingUnlockedCell property

Stellt dar, ob der Benutzer entsperrte Zellen in einem geschützten Arbeitsblatt auswählen darf.

```csharp
public bool AllowSelectingUnlockedCell { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowSelectingUnlockedCellDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Schützen Sie das Arbeitsblatt mit allen Schutzoptionen
            Protection protection = worksheet.Protection;
            
            // Setzen Sie AllowSelectingUnlockedCell auf true
            protection.AllowSelectingUnlockedCell = true;
            protection.AllowSelectingLockedCell = false;
            
            // Schutz mit Passwort anwenden
            protection.Password = "password123";
            worksheet.Protect(ProtectionType.All);

            // Überprüfen Sie die Einstellung
            Console.WriteLine("AllowSelectingUnlockedCell: " + protection.AllowSelectingUnlockedCell);
            Console.WriteLine("Worksheet is protected: " + worksheet.IsProtected);

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


