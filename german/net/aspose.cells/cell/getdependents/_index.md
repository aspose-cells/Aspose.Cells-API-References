---
title: "Cell.GetDependents"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Gibt alle Zellen zurück, deren Formel direkt auf diese Zelle verweist"
type: docs
url: /de/net/aspose.cells/cell/getdependents/
---
## Cell.GetDependents method

Ermittelt alle Zellen, deren Formel direkt auf diese Zelle verweist.

```csharp
public Cell[] GetDependents(bool isAll)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isAll | Boolean | Gibt an, ob Formeln in anderen Arbeitsblättern überprüft werden |

### Hinweise

Wenn ein Verweis, der diese Zelle enthält, in der Formel einer Zelle vorkommt, wird diese Zelle als abhängige Zelle dieser Zelle betrachtet, unabhängig davon, ob der Verweis oder diese Zelle bei der Berechnung verwendet wird oder nicht. Zum Beispiel wird die Zelle A2 in der Formel "=IF(TRUE,A1,A2)" zwar bei der Berechnung nicht verwendet, die Formel wird dennoch als abhängig von A2 angesehen. Um jene Formeln zu erhalten, deren berechnete Ergebnisse von dieser Zelle abhängen, verwenden Sie bitte [`GetDependentsInCalculation`](../getdependentsincalculation/). Beim Verfolgen von Abhängigkeiten für eine Zelle werden alle Formeln im Arbeitsbuch oder Arbeitsblatt analysiert und geprüft. Daher ist dies ein zeitaufwändiger Vorgang. Wenn der Benutzer Abhängigkeiten für viele Zellen nachverfolgen muss, führt die Verwendung dieser Methode zu schlechter Leistung. Aus Leistungsgründen sollte der Benutzer stattdessen [`GetDependentsInCalculation`](../getdependentsincalculation/) verwenden. Alternativ kann der Benutzer zunächst die Vorgänger‑Karte aller Zellen mittels [`GetPrecedents`](../getprecedents/) sammeln und dann die Abhängigkeits‑Karte anhand der Vorgänger‑Karte erstellen.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDependentsWithBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Formeln festlegen, die B1 referenzieren
            cells["A1"].Formula = "=B1+5";
            cells["A2"].Formula = "=B1*2";
            cells["A3"].Formula = "=SUM(B1:B3)";

            // Formeln berechnen
            workbook.CalculateFormula();

            // Alle Zellen abrufen, die von B1 abhängen (rekursiv)
            Cell[] dependents = cells["B1"].GetDependents(true);

            Console.WriteLine("Cells dependent on B1:");
            foreach (Cell cell in dependents)
            {
                Console.WriteLine(cell.Name + ": " + cell.Formula);
            }
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


