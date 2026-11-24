---
title: "FindOptions.GetRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FindOptions-Methode. Liest und setzt den zu suchenden Bereich"
type: docs
url: /de/net/aspose.cells/findoptions/getrange/
---
## FindOptions.GetRange method

Liest und setzt den zu suchenden Bereich.

```csharp
public CellArea GetRange()
```

### Rückgabewert

Gibt den zu suchenden Bereich zurück.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FindOptionsMethodGetRangeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einige Beispieldaten einfügen
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            worksheet.Cells["B1"].PutValue("Orange");
            worksheet.Cells["B2"].PutValue("Grape");
            worksheet.Cells["B3"].PutValue("Lemon");

            // Erstelle eine FindOptions-Instanz
            FindOptions findOptions = new FindOptions();
            findOptions.LookInType = LookInType.Values;
            findOptions.LookAtType = LookAtType.Contains;

            // Setze den Suchbereich auf A1:B3
            CellArea searchArea = new CellArea();
            searchArea.StartRow = 0;
            searchArea.StartColumn = 0;
            searchArea.EndRow = 2;
            searchArea.EndColumn = 1;
            findOptions.SetRange(searchArea);

            try
            {
                // Hole den gesetzten Bereich
                CellArea resultRange = findOptions.GetRange();

                // Zeige die Bereichsinformationen an
                Console.WriteLine($"Search range: StartRow={resultRange.StartRow}, StartColumn={resultRange.StartColumn}, " +
                    $"EndRow={resultRange.EndRow}, EndColumn={resultRange.EndColumn}");

                // Führe eine Suchoperation aus, um zu demonstrieren, dass der Bereich verwendet wird
                Cell foundCell = worksheet.Cells.Find("an", null, findOptions);
                if (foundCell != null)
                {
                    Console.WriteLine($"Found value '{foundCell.StringValue}' at {foundCell.Name}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRange method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("MethodGetRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


