---
title: "Enum FilterOperatorType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.FilterOperatorType-Enum. Benutzerdefinierter Filteroperatortyp"
type: docs
url: /de/net/aspose.cells/filteroperatortype/
---
## FilterOperatorType enumeration

Benutzerdefinierter Filteroperatortyp.

```csharp
public enum FilterOperatorType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| LessOrEqual | `0` | Stellt den LessOrEqual-Operator dar. |
| LessThan | `1` | Stellt den LessThan-Operator dar. |
| Equal | `2` | Stellt den Equal-Operator dar. |
| GreaterThan | `3` | Stellt den GreaterThan-Operator dar. |
| NotEqual | `4` | Stellt den NotEqual-Operator dar. |
| GreaterOrEqual | `5` | Stellt den GreaterOrEqual-Operator dar. |
| None | `6` | Stellt keinen Vergleich dar. |
| BeginsWith | `7` | Beginnt mit dem Text. |
| EndsWith | `8` | Endet mit dem Text. |
| Contains | `9` | Enthält den Text. |
| NotContains | `10` | Enthält den Text nicht. |
| NotBeginsWith | `11` | Beginnt nicht mit dem Text. |
| NotEndsWith | `12` | Endet nicht mit dem Text. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFilterOperatorTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Names");
            worksheet.Cells["A2"].PutValue("Bob");
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["A4"].PutValue("Bobby");
            worksheet.Cells["A5"].PutValue("Tom");
            
            // Auto-Filterbereich festlegen
            worksheet.AutoFilter.Range = "A1:A5";
            
            // Benutzerdefinierten Filter anwenden, um Namen anzuzeigen, die mit "Bo" beginnen
            worksheet.AutoFilter.Custom(0, FilterOperatorType.BeginsWith, "Bo");
            
            // Filter aktualisieren
            worksheet.AutoFilter.Refresh();
            
            // Speichere die Arbeitsmappe
            workbook.Save("FilterOperatorTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


