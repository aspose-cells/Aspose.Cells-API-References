---
title: "Cell.GetDependentsInCalculation"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Gibt alle Zellen zurück, deren berechnetes Ergebnis von dieser Zelle abhängt"
type: docs
url: /de/net/aspose.cells/cell/getdependentsincalculation/
---
## Cell.GetDependentsInCalculation method

Ermittelt alle Zellen, deren berechnetes Ergebnis von dieser Zelle abhängt.

```csharp
public IEnumerator GetDependentsInCalculation(bool recursive)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rekursiv | Boolean | Ob jene Abhängigkeiten zurückgegeben werden, die nicht direkt auf diese Zelle verweisen, sondern auf andere Blätter dieser Zelle |

### Rückgabewert

Enumerator zum Aufzählen aller Abhängigkeiten (Cell-Objekte)

### Hinweise

Um diese Methode zu verwenden, stellen Sie bitte sicher, dass das Arbeitsbuch für [`EnableCalculationChain`](../../formulasettings/enablecalculationchain/) auf den Wert true gesetzt ist und mit dieser Einstellung vollständig berechnet wurde. Wenn keine Formelbezüge zu dieser Zelle existieren, wird null zurückgegeben.

### Beispiele

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDependentsInCalculationWithBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            cells["A1"].Formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2";
            cells["A2"].Formula = "=IF(TRUE,B2,B1)";
            
            workbook.Settings.FormulaSettings.EnableCalculationChain = true;
            workbook.CalculateFormula();
            
            IEnumerator en = cells["B1"].GetDependentsInCalculation(false);
            Console.WriteLine("B1's calculation dependents:");
            while(en.MoveNext())
            {
                Cell c = (Cell)en.Current;
                Console.WriteLine(c.Name);
            }
            
            en = cells["B2"].GetDependentsInCalculation(false);
            Console.WriteLine("B2's calculation dependents:");
            while(en.MoveNext())
            {
                Cell c = (Cell)en.Current;
                Console.WriteLine(c.Name);
            }
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


