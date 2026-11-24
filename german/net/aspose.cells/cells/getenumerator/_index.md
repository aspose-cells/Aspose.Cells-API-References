---
title: "Cells.GetEnumerator"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Ruft den Zellen-Enumerator ab"
type: docs
url: /de/net/aspose.cells/cells/getenumerator/
---
## Cells.GetEnumerator method

Gibt den Zellen‑Enumerator zurück.

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
    public class CellsMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue(123);
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            
            // Enumerator abrufen und durch Zellen iterieren
            IEnumerator enumerator = worksheet.Cells.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                if (cell.Value != null)
                {
                    Console.WriteLine($"{cell.Name}: {cell.Value}");
                }
            }
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


