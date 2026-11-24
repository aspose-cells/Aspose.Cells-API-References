---
title: "ListColumn.SetCustomTotalsRowFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListColumn-Methode. Gibt die Formel der Gesamtsummen‑Zeile dieser Listenspalte zurück"
type: docs
url: /de/net/aspose.cells.tables/listcolumn/setcustomtotalsrowformula/
---
## ListColumn.SetCustomTotalsRowFormula method

Liefert die Formel der Gesamtsummenzeile dieser Listenspalte.

```csharp
public void SetCustomTotalsRowFormula(string formula, bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Formel | String | die Formel für diese Listenspalte. |
| isR1C1 | Boolean | Ob die Formel im R1C1-Format formatiert werden muss. |
| isLocal | Boolean | Ob die Formel nach den Ländereinstellungen formatiert werden muss. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnMethodSetCustomTotalsRowFormulaWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);

            // Erstelle ein Listenobjekt
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            ListObject listObject = worksheet.ListObjects[index];

            // Aktiviere die Gesamtsummen‑Zeile und setze eine benutzerdefinierte Formel
            listObject.ShowTotals = true;
            listObject.ListColumns[0].TotalsCalculation = TotalsCalculation.Custom;
            listObject.ListColumns[0].SetCustomTotalsRowFormula("=SUM([Column1])", false, false);

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


