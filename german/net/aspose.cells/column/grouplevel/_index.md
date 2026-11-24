---
title: "Column.GroupLevel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Column-Eigenschaft. Gibt die Gruppierungsebene der Spalte zurück"
type: docs
url: /de/net/aspose.cells/column/grouplevel/
---
## Column.GroupLevel property

Ermittelt die Gruppenebene der Spalte.

```csharp
public byte GroupLevel { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnPropertyGroupLevelDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Spalten gruppieren (Parameter isHidden auf false gesetzt)
            worksheet.Cells.GroupColumns(0, 2, false);
            
            // Erhalte die Gruppierungsebene der ersten Spalte
            int groupLevel = worksheet.Cells.Columns[0].GroupLevel;
            
            // Gib die Gruppierungsebene aus
            Console.WriteLine("Group level of first column: " + groupLevel);
            
            // Speichere die Arbeitsmappe
            workbook.Save("GroupLevelDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


