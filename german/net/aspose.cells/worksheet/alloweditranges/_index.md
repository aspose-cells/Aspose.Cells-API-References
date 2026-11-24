---
title: "Worksheet.AllowEditRanges"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Ruft die Sammlung der zulässigen Bearbeitungsbereiche im Arbeitsblatt ab"
type: docs
url: /de/net/aspose.cells/worksheet/alloweditranges/
---
## Worksheet.AllowEditRanges property

Liest die Sammlung der zulässigen Bearbeitungsbereiche im Arbeitsblatt.

```csharp
public ProtectedRangeCollection AllowEditRanges { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyAllowEditRangesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einen zulässigen Bearbeitungsbereich hinzu
            int index = worksheet.AllowEditRanges.Add("r1", 0, 0, 1, 1);
            ProtectedRange range = worksheet.AllowEditRanges[index];
            range.Password = "password123";

            // Schützen Sie das Arbeitsblatt
            worksheet.Protect(ProtectionType.All);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");

            // Lade die gespeicherte Arbeitsmappe zum Überprüfen
            Workbook verifyWorkbook = new Workbook("output.xlsx");
            ProtectedRange verifyRange = verifyWorkbook.Worksheets[0].AllowEditRanges[0];
            Console.WriteLine("Is protected with password: " + verifyRange.IsProtectedWithPassword);
        }
    }
}
```

### Siehe auch

* class [ProtectedRangeCollection](../../protectedrangecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


