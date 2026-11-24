---
title: "Cell.GetPrecedentsInCalculation"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Gibt alle Vorgängerreferenzen zu Zellen im aktuellen Arbeitsbuch zurück, die von der Formel dieser Zelle bei der Berechnung verwendet werden."
type: docs
url: /de/net/aspose.cells/cell/getprecedentsincalculation/
---
## Cell.GetPrecedentsInCalculation method

Liefert alle Vorgänger (Verweise auf Zellen in der aktuellen Arbeitsmappe), die von der Formel dieser Zelle bei deren Berechnung verwendet werden.

```csharp
public IEnumerator GetPrecedentsInCalculation()
```

### Rückgabewert

Enumerator zum Aufzählen aller Referenzen (ReferredArea)

### Hinweise

Diese Methode kann nur funktionieren, wenn [`EnableCalculationChain`](../../formulasettings/enablecalculationchain/) für das Arbeitsbuch auf true gesetzt ist und das Arbeitsbuch vollständig berechnet wurde. Wenn diese Zelle keine Formel ist oder keine Referenz zu anderen Zellen enthält, wird null zurückgegeben.

### Beispiele

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetPrecedentsInCalculationDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            cells["B1"].PutValue(10);
            cells["B2"].PutValue(20);
            cells["A2"].Formula = "=IF(TRUE,B2,B1)";
            
            workbook.Settings.FormulaSettings.EnableCalculationChain = true;
            workbook.CalculateFormula();
            
            IEnumerator en = cells["A2"].GetPrecedentsInCalculation();
            Console.WriteLine("A2's calculation precedents:");
            while(en.MoveNext())
            {
                ReferredArea r = (ReferredArea)en.Current;
                Console.WriteLine(r);
            }
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


