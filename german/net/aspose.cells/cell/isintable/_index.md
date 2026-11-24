---
title: "Cell.IsInTable"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Eigenschaft. Gibt an, ob diese Zelle Teil einer Tabellenformel ist"
type: docs
url: /de/net/aspose.cells/cell/isintable/
---
## Cell.IsInTable property

Gibt an, ob diese Zelle Teil einer Tabellenformel ist.

```csharp
[Obsolete("Use IsTableFormula instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsInTable { get; }
```

### Hinweise

HINWEIS: Diese Klasse ist jetzt veraltet. Verwenden Sie stattdessen Cell.IsTableFormula, um zu prüfen, ob die Zellformel Teil einer Tabellenformel ist. Diese Eigenschaft wird 12 Monate nach Mai 2018 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class CellPropertyIsInTableDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1.5);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(0.8);

            // Erstellen Sie eine Tabelle aus dem Datenbereich
            int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];

            try
            {
                // Überprüfen Sie die IsInTable‑Eigenschaft für Zellen innerhalb und außerhalb der Tabelle
                Cell cellInTable = worksheet.Cells["A2"];
                Cell cellOutsideTable = worksheet.Cells["C2"];

                Console.WriteLine("Cell A2 (inside table):");
                Console.WriteLine("  Value: " + cellInTable.StringValue);
                Console.WriteLine("  IsInTable: " + cellInTable.IsInTable);

                Console.WriteLine("\nCell C2 (outside table):");
                Console.WriteLine("  Value: " + cellOutsideTable.StringValue);
                Console.WriteLine("  IsInTable: " + cellOutsideTable.IsInTable);

                // Speichere die Arbeitsmappe
                workbook.Save("IsInTableDemo.xlsx");
                Console.WriteLine("\nWorkbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


