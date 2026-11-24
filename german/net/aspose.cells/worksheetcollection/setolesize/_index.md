---
title: "WorksheetCollection.SetOleSize"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorksheetCollection-Methode. Legt die angezeigte Größe fest, wenn die Arbeitsmappendatei als OLE-Objekt verwendet wird"
type: docs
url: /de/net/aspose.cells/worksheetcollection/setolesize/
---
## WorksheetCollection.SetOleSize method

Setzt die angezeigte Größe, wenn die Workbook-Datei als Ole-Objekt verwendet wird.

```csharp
public void SetOleSize(int startRow, int endRow, int startColumn, int endColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | Int32 | Startzeilenindex. |
| endRow | Int32 | Endzeilenindex. |
| startColumn | Int32 | Startspaltenindex. |
| endColumn | Int32 | Endspaltenindex. |

### Hinweise

Diese Methode wird allgemein verwendet, um die Anzeigegröße in PPT- oder DOC-Dateien anzupassen.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodSetOleSizeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // OLE-Größe für die Arbeitsblätter festlegen
            workbook.Worksheets.SetOleSize(0, 10, 0, 10);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
            
            // Überprüfe die OLE-Größe
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            CellArea oleSize = (CellArea)loadedWorkbook.Worksheets.OleSize;
            Console.WriteLine("OLE Size - StartRow: {0}, EndRow: {1}, StartColumn: {2}, EndColumn: {3}", 
                oleSize.StartRow, oleSize.EndRow, oleSize.StartColumn, oleSize.EndColumn);
        }
    }
}
```

### Siehe auch

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


