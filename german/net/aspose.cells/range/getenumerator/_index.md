---
title: GetEnumerator
second_title: Aspose.Cells für .NET-API-Referenz
description: Ruft den Enumerator für Zellen in diesem Bereich ab.
type: docs
weight: 300
url: /de/net/aspose.cells/range/getenumerator/
---
## Range.GetEnumerator method

Ruft den Enumerator für Zellen in diesem Bereich ab.

```csharp
public IEnumerator GetEnumerator()
```

### Rückgabewert

Der Zellenzähler

### Bemerkungen

Beim Durchlaufen von Elementen durch den zurückgegebenen Enumerator sollte die Zellensammlung nicht geändert werden (z. B. Operationen, die dazu führen, dass neue Zellen/Zeilen instanziiert oder vorhandene Zellen/Zeilen gelöscht werden). Andernfalls ist der Enumerator möglicherweise nicht in der Lage, alle Zellen korrekt zu durchlaufen (Einige Elemente können wiederholt durchlaufen oder übersprungen werden).

### Beispiele

```csharp
[C#]
Workbook workbook = new Workbook("template.xlsx");
Cells cells = workbook.Worksheets[0].Cells;

IEnumerator en = cells.CreateRange("B2:C3").GetEnumerator();
while (en.MoveNext())
{
    Cell cell = (Cell)en.Current;
    Console.WriteLine(cell.Name + ": " + cell.Value);
}
```

### Siehe auch

* class [Range](../../range)
* namensraum [Aspose.Cells](../../range)
* Montage [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
