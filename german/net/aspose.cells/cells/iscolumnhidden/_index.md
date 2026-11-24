---
title: "Cells.IsColumnHidden"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Prüft, ob eine Spalte am angegebenen Index ausgeblendet ist"
type: docs
url: /de/net/aspose.cells/cells/iscolumnhidden/
---
## Cells.IsColumnHidden method

Überprüft, ob eine Spalte am angegebenen Index ausgeblendet ist.

```csharp
public bool IsColumnHidden(int columnIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | Int32 | Spaltenindex |

### Rückgabewert

wahr, wenn die Spalte ausgeblendet ist.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodIsColumnHiddenWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Spalte C ausblenden (Index 2)
            cells.HideColumn(2);
            
            // Prüfen, ob Spalte C ausgeblendet ist
            bool isHidden = cells.IsColumnHidden(2);
            
            Console.WriteLine("Is column C (index 2) hidden? " + isHidden);
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


