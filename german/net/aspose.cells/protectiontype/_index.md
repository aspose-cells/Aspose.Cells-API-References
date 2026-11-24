---
title: "Enum ProtectionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ProtectionType enum. Gibt den Schutztyp für Arbeitsmappe/Arbeitsblatt an"
type: docs
url: /de/net/aspose.cells/protectiontype/
---
## ProtectionType enumeration

Stellt den Schutztyp für Arbeitsmappe/Arbeitsblatt dar.

```csharp
public enum ProtectionType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| All | `0` | Stellt dar, alles zu schützen. |
| Contents | `1` | Stellt dar, Inhalte zu schützen, verwendet im Arbeitsblattschutz. |
| Objects | `2` | Stellt dar, Objekte zu schützen, verwendet im Arbeitsblattschutz. |
| Scenarios | `3` | Stellt dar, Szenarien zu schützen, verwendet im Arbeitsblattschutz. |
| Structure | `4` | Stellt dar, die Struktur zu schützen, verwendet im Schutz der Arbeitsmappe. |
| Windows | `5` | Stellt dar, das Fenster zu schützen, verwendet im Schutz der Arbeitsmappe. |
| None | `6` | Stellt keinen Schutz dar. Nur für die Lese‑Eigenschaft. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassProtectionTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Schützen Sie das Arbeitsblatt mit allen Schutzarten
            worksheet.Protect(ProtectionType.All);
            
            // Demonstriert den Zugriff auf Schutzeigenschaften
            Console.WriteLine("Worksheet protection settings:");
            Console.WriteLine("AllowDeletingColumn: " + worksheet.Protection.AllowDeletingColumn);
            Console.WriteLine("AllowDeletingRow: " + worksheet.Protection.AllowDeletingRow);
            Console.WriteLine("AllowFiltering: " + worksheet.Protection.AllowFiltering);
            Console.WriteLine("AllowFormattingCell: " + worksheet.Protection.AllowFormattingCell);
            Console.WriteLine("AllowFormattingColumn: " + worksheet.Protection.AllowFormattingColumn);
            Console.WriteLine("AllowFormattingRow: " + worksheet.Protection.AllowFormattingRow);
            Console.WriteLine("AllowInsertingColumn: " + worksheet.Protection.AllowInsertingColumn);
            Console.WriteLine("AllowInsertingHyperlink: " + worksheet.Protection.AllowInsertingHyperlink);
            Console.WriteLine("AllowInsertingRow: " + worksheet.Protection.AllowInsertingRow);
            Console.WriteLine("AllowSorting: " + worksheet.Protection.AllowSorting);
            Console.WriteLine("AllowUsingPivotTable: " + worksheet.Protection.AllowUsingPivotTable);
            
            // Entfernen Sie den Schutz des Arbeitsblatts
            worksheet.Unprotect();
            
            // Schützen mit bestimmten Schutzarten
            worksheet.Protect(ProtectionType.Contents | ProtectionType.Objects);
            Console.WriteLine("\nWorksheet protected with Contents and Objects only");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


