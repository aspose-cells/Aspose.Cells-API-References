---
title: "Worksheet.UnFreezePanes"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Hebt die Fixierung von Bereichen im Arbeitsblatt auf"
type: docs
url: /de/net/aspose.cells/worksheet/unfreezepanes/
---
## Worksheet.UnFreezePanes method

Löst das Einfrieren von Bereichen im Arbeitsblatt auf.

```csharp
public void UnFreezePanes()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodUnFreezePanesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Bereiche bei Zelle C3 fixieren (Zeilen 2, Spalten 2 fixiert)
            worksheet.FreezePanes("C3", 2, 2);

            // Überprüfen, ob Bereiche fixiert sind
            int frozenRow, frozenColumn, frozenRows, frozenColumns;
            worksheet.GetFreezedPanes(out frozenRow, out frozenColumn, out frozenRows, out frozenColumns);
            Console.WriteLine($"Frozen panes - Row: {frozenRow}, Column: {frozenColumn}, Rows: {frozenRows}, Columns: {frozenColumns}");

            // Bereiche wieder lösen
            worksheet.UnFreezePanes();

            // Überprüfen, ob Bereiche nicht mehr fixiert sind
            worksheet.GetFreezedPanes(out frozenRow, out frozenColumn, out frozenRows, out frozenColumns);
            Console.WriteLine($"After UnFreezePanes - Row: {frozenRow}, Column: {frozenColumn}, Rows: {frozenRows}, Columns: {frozenColumns}");

            // Speichere die Arbeitsmappe
            workbook.Save("UnFreezePanesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


