---
title: "ListColumn.GetCustomTotalsRowFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListColumn-Methode. Gibt die Formel der Gesamtsummen‑Zeile dieser Listenspalte zurück"
type: docs
url: /de/net/aspose.cells.tables/listcolumn/getcustomtotalsrowformula/
---
## ListColumn.GetCustomTotalsRowFormula method

Liefert die Formel der Gesamtsummenzeile dieser Listenspalte.

```csharp
public string GetCustomTotalsRowFormula(bool isR1C1, bool isLocal)
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
    public class ListColumnMethodGetCustomTotalsRowFormulaWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);

            // Erstelle ein Listenobjekt
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            ListObject listObject = worksheet.ListObjects[index];

            // Setze benutzerdefinierte Gesamtsummen‑Formel
            ListColumn listColumn = listObject.ListColumns[0];
            listColumn.TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Custom;
            listColumn.SetCustomTotalsRowFormula("=SUM([Column1])", false, false);

            // Rufe die benutzerdefinierte Gesamtsummen‑Formel ab und zeige sie an
            string formula = listColumn.GetCustomTotalsRowFormula(false, true);
            Console.WriteLine("Custom Totals Formula: " + formula);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


