---
title: "ValidationCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ValidationCollection-Eigenschaft. Gibt das Validation-Element am angegebenen Index zurück"
type: docs
url: /de/net/aspose.cells/validationcollection/item/
---
## ValidationCollection indexer

Gibt das [`Validation`](../../validation/) Element am angegebenen Index zurück.

```csharp
public Validation this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der nullbasierte Index des Elements. |

### Rückgabewert

Das Element am angegebenen Index.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie den Zellen eine Datenvalidierung hinzu
            ValidationCollection validations = sheet.Validations;
            
            // Erster Validierungsbereich
            Validation validation1 = validations[validations.Add()];
            validation1.AddArea(new CellArea { StartRow = 1, StartColumn = 1, EndRow = 4, EndColumn = 3 });
            
            // Zweiter Validierungsbereich
            Validation validation2 = validations[validations.Add()];
            validation2.AddArea(new CellArea { StartRow = 6, StartColumn = 1, EndRow = 6, EndColumn = 3 });

            // Greifen Sie über die Item-Eigenschaft auf die Validierung zu
            Validation firstValidation = validations[0];
            Console.WriteLine($"First validation has {firstValidation.Areas.Length} area(s)");

            // Bereiche überprüfen
            foreach (CellArea area in firstValidation.Areas)
            {
                Console.WriteLine($"Area: {area.StartRow},{area.StartColumn} to {area.EndRow},{area.EndColumn}");
            }
        }
    }
}
```

### Siehe auch

* class [Validation](../../validation/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


