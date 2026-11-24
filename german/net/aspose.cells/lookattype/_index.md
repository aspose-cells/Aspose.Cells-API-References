---
title: "Aufzählung LookAtType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.LookAtType-Enum. Stellt den Suchtyp dar"
type: docs
url: /de/net/aspose.cells/lookattype/
---
## LookAtType enumeration

Stellt den Typ 'look at' dar.

```csharp
public enum LookAtType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Contains | `0` | Zellwert enthält das Suchobjekt. |
| StartWith | `1` | Zellwert beginnt mit dem Suchobjekt. |
| EndWith | `2` | Zellwert endet mit dem Suchobjekt. |
| EntireContent | `3` | Zellwert ist derselbe wie das Suchobjekt. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LookAtTypeDemo
    {
        public static void LookAtTypeExample()
        {
            // Instanziieren Sie das Arbeitsmappen-Objekt
            Workbook workbook = new Workbook("LookAtTypeExample_original.xlsx");

            // Abrufen der Zellen-Sammlung
            Cells cells = workbook.Worksheets[0].Cells;

            // Instanziieren Sie das FindOptions-Objekt
            FindOptions findOptions = new FindOptions();

            // Erstellen Sie einen Zellenbereich
            CellArea ca = new CellArea();
            ca.StartRow = 8;
            ca.StartColumn = 2;
            ca.EndRow = 17;
            ca.EndColumn = 13;

            // Legen Sie den Zellenbereich für FindOptions fest
            findOptions.SetRange(ca);

            // Such-Eigenschaften festlegen
            findOptions.SearchBackward = false;
            findOptions.SearchOrderByRows = true;
            findOptions.LookInType = LookInType.Values;

            // Setzen Sie LookAtType auf Contains
            findOptions.LookAtType = LookAtType.Contains;

            // Suchen Sie die Zelle mit einem bestimmten Wert
            Cell cell = cells.Find("searchValue", null, findOptions);

            if (cell != null)
            {
                Console.WriteLine($"Cell found at row {cell.Row}, column {cell.Column}");
            }
            else
            {
                Console.WriteLine("Cell not found.");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


