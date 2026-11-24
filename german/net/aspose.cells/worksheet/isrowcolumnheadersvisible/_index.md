---
title: "Worksheet.IsRowColumnHeadersVisible"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Ruft einen Wert ab oder legt ihn fest, der angibt, ob das Arbeitsblatt Zeilen- und Spaltenüberschriften anzeigt. Standard ist true"
type: docs
url: /de/net/aspose.cells/worksheet/isrowcolumnheadersvisible/
---
## Worksheet.IsRowColumnHeadersVisible property

Liest oder setzt einen Wert, der angibt, ob das Arbeitsblatt Zeilen- und Spaltenüberschriften anzeigt. Standard ist true.

```csharp
public bool IsRowColumnHeadersVisible { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsRowColumnHeadersVisibleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setzen Sie die Sichtbarkeit von Zeilen- und Spaltenüberschriften auf false
            worksheet.IsRowColumnHeadersVisible = false;
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
            
            // Laden Sie die gespeicherte Arbeitsmappe, um die Eigenschaft zu überprüfen
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Geben Sie den Eigenschaftswert aus
            Console.WriteLine("Row and Column Headers Visible: " + loadedWorksheet.IsRowColumnHeadersVisible);
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


