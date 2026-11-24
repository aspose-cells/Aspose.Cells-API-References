---
title: "ListColumn.IsArrayFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListColumn-Eigenschaft. Gibt an, ob die Formel eine Array-Formel ist"
type: docs
url: /de/net/aspose.cells.tables/listcolumn/isarrayformula/
---
## ListColumn.IsArrayFormula property

Gibt an, ob die Formel eine Array-Formel ist.

```csharp
public bool IsArrayFormula { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListColumnPropertyIsArrayFormulaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten hinzu, um eine Tabelle zu erstellen
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue(20);

            // Ein Tabellen-/Listenobjekt erstellen
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[tableIndex];

            // Füge der zweiten Spalte eine Array-Formel hinzu
            listObject.ListColumns[1].Formula = "{=SUM(A2:A3*B2:B3)}";

            try
            {
                // Greife auf die IsArrayFormula-Eigenschaft zu (schreibgeschützt)
                bool isArrayFormula = listObject.ListColumns[1].IsArrayFormula;

                // Wert anzeigen
                Console.WriteLine("IsArrayFormula value: " + isArrayFormula);

                // Speichere die Arbeitsmappe
                workbook.Save("IsArrayFormulaDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
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

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


