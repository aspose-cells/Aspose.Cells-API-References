---
title: "ListColumn.GetCustomCalculatedFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListColumn-Methode. Gibt die Formel dieser Listenspalte zurück"
type: docs
url: /de/net/aspose.cells.tables/listcolumn/getcustomcalculatedformula/
---
## ListColumn.GetCustomCalculatedFormula method

Liefert die Formel dieser Listenspalte.

```csharp
public string GetCustomCalculatedFormula(bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isR1C1 | Boolean | Ob die Formel im R1C1-Format formatiert werden muss. |
| isLocal | Boolean | Ob die Formel nach den Ländereinstellungen formatiert werden muss. |

### Rückgabewert

Die Formel dieser Listenspalte.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnMethodGetCustomCalculatedFormulaWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Erstelle Beispieldaten
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["A3"].PutValue("Mary");
            sheet.Cells["B1"].PutValue("Score");
            sheet.Cells["B2"].PutValue(85);
            sheet.Cells["B3"].PutValue(92);
            
            // Erstelle ein Listenobjekt
            int index = sheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = sheet.ListObjects[index];
            
            // Füge eine berechnete Spalte hinzu
            ListColumn calcColumn = listObject.ListColumns[1];
            calcColumn.Formula = "=WEEKNUM([@Score])";
            
            // Rufe die benutzerdefinierte berechnete Formel ab
            string formula = listObject.ListColumns[1].GetCustomCalculatedFormula(false, false);
            
            // Gib das Ergebnis aus
            Console.WriteLine("Calculated Formula: " + formula);
        }
    }
}
```

### Siehe auch

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


