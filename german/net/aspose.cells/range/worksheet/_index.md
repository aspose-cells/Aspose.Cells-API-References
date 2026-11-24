---
title: "Range.Worksheet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Eigenschaft. Gibt das Worksheet-Objekt zurück, das diesen Bereich enthält"
type: docs
url: /de/net/aspose.cells/range/worksheet/
---
## Range.Worksheet property

Gibt das `Worksheet`-Objekt zurück, das diesen Bereich enthält.

```csharp
public Worksheet Worksheet { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyWorksheetDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Benannten Bereich erstellen
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["B1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            
            // Definieren Sie einen benannten Bereich
            int index = workbook.Worksheets.Names.Add("MyRange");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!$A$1:$B$2";
            
            // Rufen Sie den Bereich nach Namen ab (qualifizieren Sie Range vollständig, um Mehrdeutigkeiten zu vermeiden)
            Aspose.Cells.Range range = workbook.Worksheets.GetRangeByName("MyRange");
            
            // Veranschaulichen Sie die Verwendung der Worksheet-Eigenschaft
            Console.WriteLine("Range belongs to worksheet: " + range.Worksheet.Name);
            
            // Verwenden Sie die Worksheet-Eigenschaft, um Zellen zu ändern
            range.Worksheet.Cells["A1"].PutValue("Updated");
            
            // Speichere die Arbeitsmappe
            workbook.Save("RangePropertyWorksheetDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../../worksheet/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


