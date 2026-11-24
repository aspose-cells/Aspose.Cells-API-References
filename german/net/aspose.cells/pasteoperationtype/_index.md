---
title: "Enum PasteOperationType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.PasteOperationType Enum. Stellt den Operationstyp beim Einfügen eines Bereichs dar"
type: docs
url: /de/net/aspose.cells/pasteoperationtype/
---
## PasteOperationType enumeration

Stellt den Vorgangstyp beim Einfügen eines Bereichs dar.

```csharp
public enum PasteOperationType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Keine Operation. |
| Add | `1` | Hinzufügen |
| Subtract | `2` | Subtrahieren |
| Multiply | `3` | Multiplizieren |
| Divide | `4` | Dividieren |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassPasteOperationTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Füge Beispieldaten zu Zellen hinzu
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["B1"].PutValue(20);
            sheet.Cells["C1"].PutValue(30);
            
            // Erstelle Einfügeoptionen mit PasteOperationType.None
            var pasteOptions = new PasteOptions()
            {
                PasteType = PasteType.Values,
                OperationType = PasteOperationType.None,
                SkipBlanks = false,
                Transpose = false
            };

            // Erstelle einen Bereich und kopiere mit Einfügeoptionen
            Aspose.Cells.Range sourceRange = sheet.Cells.CreateRange("A1", "C1");
            Aspose.Cells.Range destRange = sheet.Cells.CreateRange("A2", "C2");
            sourceRange.Copy(destRange, pasteOptions);

            // Speichere die Arbeitsmappe
            workbook.Save("PasteOperationTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


