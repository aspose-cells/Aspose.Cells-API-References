---
title: "Cells.GetDependentsInCalculation"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells‑Methode. Gibt alle Zellen zurück, deren berechnetes Ergebnis von einer bestimmten Zelle abhängt."
type: docs
url: /de/net/aspose.cells/cells/getdependentsincalculation/
---
## Cells.GetDependentsInCalculation method

Gibt alle Zellen zurück, deren berechnetes Ergebnis von einer bestimmten Zelle abhängt.

```csharp
public IEnumerator GetDependentsInCalculation(int row, int column, bool recursive)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex der spezifischen Zelle |
| column | Int32 | Spaltenindex der spezifischen Zelle. |
| rekursiv | Boolean | Ob diejenigen Abhängigkeiten zurückgegeben werden, die nicht direkt auf die spezifische Zelle verweisen, sondern auf andere Blätter dieser Zelle. |

### Rückgabewert

Enumerator zum Aufzählen aller Abhängigkeiten (Cell-Objekte)

### Hinweise

Um diese Methode zu verwenden, stellen Sie bitte sicher, dass das Arbeitsbuch den Wert true für [`EnableCalculationChain`](../../formulasettings/enablecalculationchain/) gesetzt hat und mit dieser Einstellung vollständig berechnet wurde. Wenn keine Formelbeziehung zu dieser Zelle besteht, wird null zurückgegeben. Weitere Details und ein Beispiel finden Sie unter [`GetDependentsInCalculation`](../../cell/getdependentsincalculation/).

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsMethodGetDependentsInCalculationWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Erstellen Sie ein neues Arbeitsbuch und berechnen Sie Formeln
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Richten Sie Formelbeziehungen ein:
            // C1 = 10 (Quellwert)
            // B1 = C1*2
            // A1 = B1+5
            cells["C1"].PutValue(10);
            cells["B1"].Formula = "C1*2";
            cells["A1"].Formula = "B1+5";

            // Berechnen Sie Formeln, um Abhängigkeiten herzustellen
            workbook.CalculateFormula();

            try
            {
                // Abrufen der Abhängigkeiten für Zelle C1 (Zeile 0, Spalte 2) mit rekursiver Prüfung
                IEnumerator dependents = cells.GetDependentsInCalculation(0, 2, true);

                Console.WriteLine("Dependents of cell C1:");
                while (dependents.MoveNext())
                {
                    if (dependents.Current is Cell dependentCell)
                    {
                        Console.WriteLine($"- {dependentCell.Name}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetDependentsInCalculation: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("GetDependentsInCalculationDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


