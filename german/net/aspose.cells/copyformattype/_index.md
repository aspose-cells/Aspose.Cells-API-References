---
title: "Enum CopyFormatType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.CopyFormatType Enum. Stellt den Typ des Kopierformats beim Einfügen von Zeilen dar"
type: docs
url: /de/net/aspose.cells/copyformattype/
---
## CopyFormatType enumeration

Stellt den Typ des Kopierformats beim Einfügen von Zeilen dar.

```csharp
public enum CopyFormatType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| SameAsAbove | `0` | Formatiert wie die darüberliegende Zeile. |
| SameAsBelow | `1` | Formatiert wie die darunterliegende Zeile. |
| Clear | `2` | Löscht die Formatierung. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CopyFormatTypeDemo
    {
        public static void CopyFormatTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füllen Sie einige Daten im Arbeitsblatt ein
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");

            // Erstelle InsertOptions und setze CopyFormatType
            InsertOptions insertOptions = new InsertOptions();
            insertOptions.CopyFormatType = CopyFormatType.SameAsAbove;

            // Füge an der zweiten Position eine Zeile mit dem angegebenen Formattyp ein
            worksheet.Cells.InsertRows(1, 1, insertOptions);

            // Speichere die Arbeitsmappe
            workbook.Save("CopyFormatTypeExample.xlsx");
            workbook.Save("CopyFormatTypeExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


