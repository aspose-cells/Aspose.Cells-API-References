---
title: "Protection.AllowDeletingColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Protection-Eigenschaft. Gibt an, ob das Löschen von Spalten in einem geschützten Arbeitsblatt erlaubt ist."
type: docs
url: /de/net/aspose.cells/protection/allowdeletingcolumn/
---
## Protection.AllowDeletingColumn property

Stellt dar, ob das Löschen von Spalten in einem geschützten Arbeitsblatt erlaubt ist.

```csharp
public bool AllowDeletingColumn { get; set; }
```

### Hinweise

Die Spalten, die die zu löschenden Zellen enthalten, müssen beim geschützten Blatt entsperrt sein, und die Option "Entsperrte Zellen auswählen" muss aktiviert sein.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowDeletingColumnDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Arbeitsblattschutz aktivieren
            Protection protection = worksheet.Protection;
            protection.AllowDeletingColumn = true;
            worksheet.Protect(ProtectionType.All);

            // Überprüfen Sie die Einstellung
            Console.WriteLine("AllowDeletingColumn: " + protection.AllowDeletingColumn);

            // Versuchen Sie, eine Spalte zu löschen (sollte funktionieren, da AllowDeletingColumn true ist)
            worksheet.Cells.DeleteColumn(0);
            Console.WriteLine("Column deleted successfully");

            // Spaltenlöschung deaktivieren
            protection.AllowDeletingColumn = false;

            // Versuchen Sie, eine weitere Spalte zu löschen (sollte fehlschlagen)
            try
            {
                worksheet.Cells.DeleteColumn(1);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Failed to delete column: " + ex.Message);
            }
        }
    }
}
```

### Siehe auch

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


