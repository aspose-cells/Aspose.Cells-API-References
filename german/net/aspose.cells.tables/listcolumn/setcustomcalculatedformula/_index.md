---
title: "ListColumn.SetCustomCalculatedFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListColumn-Methode. Legt die Formel für diese Listenspalte fest"
type: docs
url: /de/net/aspose.cells.tables/listcolumn/setcustomcalculatedformula/
---
## ListColumn.SetCustomCalculatedFormula method

Setzt die Formel für diese Listenspalte.

```csharp
public void SetCustomCalculatedFormula(string formula, bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Formel | String | die Formel für diese Listenspalte. |
| isR1C1 | Boolean | Ob die Formel im R1C1-Format formatiert werden muss. |
| isLocal | Boolean | Ob die Formel nach den Ländereinstellungen formatiert werden muss. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListColumnMethodSetCustomCalculatedFormulaWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für die Tabelle erstellen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B1"].PutValue("Total");

            // Tabelle erstellen
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true); // Adjusted parameters to match correct overload
            ListObject table = worksheet.ListObjects[tableIndex];

            // Zweite Listenspalte abrufen
            ListColumn totalColumn = table.ListColumns[1];

            try
            {
                // Benutzerdefinierte Formel mit A1-Notation und Standard-Locale festlegen
                totalColumn.SetCustomCalculatedFormula("=A2*1.1", false, false);
                
                Console.WriteLine("Custom formula set successfully.");
                Console.WriteLine($"Cell B2 formula: {worksheet.Cells["B2"].Formula}");
                Console.WriteLine($"Cell B3 formula: {worksheet.Cells["B3"].Formula}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("SetCustomCalculatedFormulaExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


