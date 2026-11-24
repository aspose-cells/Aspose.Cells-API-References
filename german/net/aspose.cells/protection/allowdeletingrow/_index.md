---
title: "Protection.AllowDeletingRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Protection-Eigenschaft. Gibt an, ob das Löschen von Zeilen in einem geschützten Arbeitsblatt erlaubt ist."
type: docs
url: /de/net/aspose.cells/protection/allowdeletingrow/
---
## Protection.AllowDeletingRow property

Stellt dar, ob das Löschen von Zeilen in einem geschützten Arbeitsblatt erlaubt ist.

```csharp
public bool AllowDeletingRow { get; set; }
```

### Hinweise

Die Zeilen, die die zu löschenden Zellen enthalten, müssen entsperrt sein, wenn das Blatt geschützt ist, und die Option "Entsperrte Zellen auswählen" muss aktiviert sein.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowDeletingRowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Schutzeinstellungen festlegen
            Protection protection = sheet.Protection;
            protection.AllowDeletingRow = true;
            protection.AllowSorting = true;
            protection.AllowFiltering = true;
            protection.AllowFormattingColumn = true;

            // Schützen Sie das Arbeitsblatt
            sheet.Protect(ProtectionType.All);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");

            // Laden Sie die gespeicherte Arbeitsmappe, um die Einstellungen zu überprüfen
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedSheet = loadedWorkbook.Worksheets[0];

            // Verifiziere AllowDeletingRow und andere Eigenschaften
            Console.WriteLine("AllowDeletingRow: " + loadedSheet.Protection.AllowDeletingRow);
            Console.WriteLine("AllowSorting: " + loadedSheet.Protection.AllowSorting);
            Console.WriteLine("AllowFiltering: " + loadedSheet.Protection.AllowFiltering);
            Console.WriteLine("AllowFormattingColumn: " + loadedSheet.Protection.AllowFormattingColumn);
        }
    }
}
```

### Siehe auch

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


