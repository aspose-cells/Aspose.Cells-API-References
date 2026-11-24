---
title: "Worksheet.ConvertFormulaReferenceStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Konvertiert den Formel-Referenzstil"
type: docs
url: /de/net/aspose.cells/worksheet/convertformulareferencestyle/
---
## Worksheet.ConvertFormulaReferenceStyle method

Konvertiert den Formel-Referenzstil.

```csharp
public string ConvertFormulaReferenceStyle(string formula, bool toR1C1, int baseCellRow, 
    int baseCellColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Formel | String | Die zu konvertierende Formel. |
| toR1C1 | Boolean | Welcher Referenzstil für die Konvertierung der Formel verwendet werden soll. Wenn die ursprüngliche Formel im A1‑Referenzstil vorliegt, sollte dieser Wert true sein, damit die Formel vom A1‑ in den R1C1‑Referenzstil konvertiert wird; wenn die ursprüngliche Formel im R1C1‑Referenzstil vorliegt, sollte dieser Wert false sein, damit die Formel vom R1C1‑ in den A1‑Referenzstil konvertiert wird; |
| baseCellRow | Int32 | Der Zeilenindex der Basiszelle. |
| baseCellColumn | Int32 | Der Spaltenindex der Basiszelle. |

### Rückgabewert

Die konvertierte Formel.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodConvertFormulaReferenceStyleWithStringBooleanInt32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Beispiel 1: R1C1‑Stil in A1‑Stil konvertieren
            string formulaR1C1 = "R[0]C23,testDS,R[0]C24";
            string formulaA1 = sheet.ConvertFormulaReferenceStyle(formulaR1C1, false, 0, 0);
            Console.WriteLine("Converted formula: " + formulaA1);

            // Beispiel 2: Mit gemischten Referenzen konvertieren
            string formulaMixed = "R[0]C23,testDS,rcurr,R[0]C24";
            string convertedMixed = sheet.ConvertFormulaReferenceStyle(formulaMixed, false, 0, 0);
            Console.WriteLine("Converted mixed formula: " + convertedMixed);
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


