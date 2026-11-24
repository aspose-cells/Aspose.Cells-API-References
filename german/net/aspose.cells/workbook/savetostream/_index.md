---
title: "Workbook.SaveToStream"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook‑Methode. Speichert die Excel‑Datei in ein MemoryStream‑Objekt als Excel972003‑xls‑Datei und gibt sie zurück"
type: docs
url: /de/net/aspose.cells/workbook/savetostream/
---
## Workbook.SaveToStream method

Speichert die Excel-Datei in ein MemoryStream-Objekt als Excel97-2003 xls-Datei und gibt sie zurück.

```csharp
public MemoryStream SaveToStream()
```

### Rückgabewert

MemoryStream‑Objekt, das eine xls‑Excel‑Datei enthält.

### Hinweise

Diese Methode bietet dieselbe Funktion wie die Save‑Methode und speichert die Arbeitsmappe nur als Excel97‑2003‑xls‑Datei. Sie ist hauptsächlich für Aufrufe von COM‑Clients gedacht.

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveToStreamDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook start = new Workbook();
            
            // Greifen Sie auf das erste Arbeitsblatt zu und fügen Sie Beispieldaten hinzu.
            Worksheet worksheet = start.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // Arbeitsmappe in MemoryStream speichern
            MemoryStream stream = start.SaveToStream();

            // Neue Arbeitsmappe aus dem Stream erstellen
            Workbook workbook = new Workbook(stream);

            // Neue Arbeitsmappe bearbeiten
            Worksheet newWorksheet = workbook.Worksheets[0];
            var area = CellArea.CreateCellArea(3, 0, 3, 1);
            newWorksheet.Cells.InsertRange(area, 3, ShiftType.Down, true);

            newWorksheet.Cells["A4"].PutValue("D");
            newWorksheet.Cells["B4"].PutValue(40);
            newWorksheet.Cells["A5"].PutValue("E");
            newWorksheet.Cells["B5"].PutValue(50);
            newWorksheet.Cells["A6"].PutValue("F");
            newWorksheet.Cells["B6"].PutValue(60);

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


