---
title: "ProtectedRangeCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ProtectedRangeCollection-Eigenschaft. Gibt das ProtectedRange-Element am angegebenen Index zurück"
type: docs
url: /de/net/aspose.cells/protectedrangecollection/item/
---
## ProtectedRangeCollection indexer

Gibt das [`ProtectedRange`](../../protectedrange/)‑Element am angegebenen Index zurück.

```csharp
public ProtectedRange this[int index] { get; }
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
    public class ProtectedRangeCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge einen geschützten Bereich mithilfe von Zellindizes hinzu (startRow, startColumn, endRow, endColumn)
            int index = worksheet.AllowEditRanges.Add("MyProtectedRange", 0, 0, 1, 1);
            ProtectedRange protectedRange = worksheet.AllowEditRanges[index];
            protectedRange.Password = "password123";
            
            // Greife auf den geschützten Bereich über die Item‑Eigenschaft zu (Index 0)
            ProtectedRange retrievedRange = worksheet.AllowEditRanges[0];
            
            // Überprüfe und zeige den Schutzstatus an
            Console.WriteLine("Is protected with password: " + retrievedRange.IsProtectedWithPassword);
            Console.WriteLine("Range name: " + retrievedRange.Name);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ProtectedRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ProtectedRange](../../protectedrange/)
* class [ProtectedRangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


