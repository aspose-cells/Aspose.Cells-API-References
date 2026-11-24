---
title: "AutoFilter.Filter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AutoFilter-Methode. Filtert eine Liste nach angegebenen Kriterien"
type: docs
url: /de/net/aspose.cells/autofilter/filter/
---
## AutoFilter.Filter method

Filtert eine Liste mit angegebenen Kriterien.

```csharp
public void Filter(int fieldIndex, string criteria)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldIndex | Int32 | Der ganzzahlige Versatz des Feldes, auf dem der Filter basieren soll (vom linken Rand der Liste; das linkeste Feld ist Feld 0). |
| Kriterien | String | Das angegebene Kriterium (ein String; zum Beispiel "101"). |

### Hinweise

Aspose.Cells entfernt alle anderen Filtereinstellungen für dieses Feld wie in MS Excel 97-2003.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodFilterWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("Nom1");
            sheet.Cells["A3"].PutValue("Nom2");
            sheet.Cells["A4"].PutValue("Nom3");
            sheet.Cells["A5"].PutValue("Nom2");

            // Wende AutoFilter mit korrekten SetRange-Parametern an
            sheet.AutoFilter.SetRange(0, 0, 4); // startRow: 0, startColumn: 0, endRow: 4
            sheet.AutoFilter.Filter(0, "Nom2"); // Filter column 0 (A) for "Nom2"
            sheet.AutoFilter.Refresh();

            // Ergebnis speichern
            workbook.Save("AutoFilterDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


