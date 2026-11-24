---
title: "FindOptions.IsRangeSet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FindOptions-Eigenschaft. Gibt an, ob der zu suchende Bereich festgelegt ist"
type: docs
url: /de/net/aspose.cells/findoptions/israngeset/
---
## FindOptions.IsRangeSet property

Gibt an, ob der gesuchte Bereich festgelegt ist.

```csharp
public bool IsRangeSet { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FindOptionsPropertyIsRangeSetDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einige Daten befüllen
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            worksheet.Cells["B1"].PutValue("Date");
            worksheet.Cells["B2"].PutValue("Elderberry");
            worksheet.Cells["B3"].PutValue("Fig");

            // Erstelle eine FindOptions-Instanz
            FindOptions findOptions = new FindOptions();

            // Überprüfe den anfänglichen IsRangeSet-Wert (sollte false sein)
            Console.WriteLine("Initial IsRangeSet value: " + findOptions.IsRangeSet);

            // Setze einen Suchbereich
            CellArea searchRange = new CellArea();
            searchRange.StartRow = 0;
            searchRange.StartColumn = 0;
            searchRange.EndRow = 2;
            searchRange.EndColumn = 0; // Column A only
            findOptions.SetRange(searchRange);

            // Überprüfe IsRangeSet nach dem Festlegen des Bereichs (sollte true sein)
            Console.WriteLine("After SetRange, IsRangeSet value: " + findOptions.IsRangeSet);

            // Führe eine Suchoperation innerhalb des angegebenen Bereichs aus
            Cell foundCell = worksheet.Cells.Find("Banana", null, findOptions);
            Console.WriteLine("Found 'Banana' at: " + foundCell?.Name);

            // Versuche, etwas außerhalb des Bereichs zu finden (sollte nicht gefunden werden)
            foundCell = worksheet.Cells.Find("Fig", null, findOptions);
            Console.WriteLine("Found 'Fig' at: " + foundCell?.Name); // Should be null

            // Speichere die Arbeitsmappe
            workbook.Save("PropertyIsRangeSetDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


