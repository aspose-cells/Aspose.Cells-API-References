---
title: "Workbook.Worksheets"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Eigenschaft. Gibt die WorksheetCollection‑Sammlung im Tabellenblatt zurück"
type: docs
url: /de/net/aspose.cells/workbook/worksheets/
---
## Workbook.Worksheets property

Gibt die [`WorksheetCollection`](../../worksheetcollection/)‑Sammlung im Tabellenblatt zurück.

```csharp
public WorksheetCollection Worksheets { get; }
```

### Rückgabewert

[`WorksheetCollection`](../../worksheetcollection/) collection

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyWorksheetsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            
            // Ein neues Arbeitsblatt hinzufügen
            workbook.Worksheets.Add("SecondSheet");
            
            // Greife auf das zweite Arbeitsblatt zu und füge Daten hinzu
            Worksheet secondSheet = workbook.Worksheets[1];
            secondSheet.Cells["A1"].PutValue("Product");
            secondSheet.Cells["B1"].PutValue("Price");
            secondSheet.Cells["A2"].PutValue("Laptop");
            secondSheet.Cells["B2"].PutValue(999.99);
            
            // Speichere die Arbeitsmappe
            workbook.Save("WorkbookWorksheetsDemo.xlsx");
            
            // Ausgabe der Arbeitsblattanzahl
            Console.WriteLine($"Number of worksheets: {workbook.Worksheets.Count}");
        }
    }
}
```

### Siehe auch

* class [WorksheetCollection](../../worksheetcollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


