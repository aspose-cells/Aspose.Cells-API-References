---
title: "Range.GetEnumerator"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Gibt den Enumerator für Zellen in diesem Range zurück"
type: docs
url: /de/net/aspose.cells/range/getenumerator/
---
## Range.GetEnumerator method

Ruft den Enumerator für Zellen in diesem Range ab.

```csharp
public IEnumerator GetEnumerator()
```

### Rückgabewert

Der Zellen-Enumerator

### Hinweise

Beim Durchlaufen von Elementen mit dem zurückgegebenen Enumerator sollte die Zellen-Sammlung nicht verändert werden (z. B. Vorgänge, die dazu führen, dass neue Cell/Row instanziiert oder vorhandene Cell/Row gelöscht werden). Andernfalls kann der Enumerator möglicherweise nicht alle Zellen korrekt durchlaufen (einige Elemente könnten mehrfach durchlaufen oder übersprungen werden).

### Beispiele

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Einige Beispieldaten einfügen
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["B3"].PutValue("Banana");
            worksheet.Cells["C2"].PutValue("Cherry");
            worksheet.Cells["C3"].PutValue("Date");

            // Bereich abrufen und durch Zellen enumerieren
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C3");
            IEnumerator enumerator = range.GetEnumerator();
            
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                Console.WriteLine($"{cell.Name}: {cell.Value}");
            }
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


