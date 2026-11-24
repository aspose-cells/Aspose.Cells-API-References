---
title: "ProtectedRangeCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ProtectedRangeCollection-Methode. Fügt ein ProtectedRange-Element zur Sammlung hinzu"
type: docs
url: /de/net/aspose.cells/protectedrangecollection/add/
---
## ProtectedRangeCollection.Add method

Fügt ein [`ProtectedRange`](../../protectedrange/) Element zur Sammlung hinzu.

```csharp
public int Add(string name, int startRow, int startColumn, int endRow, int endColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | Bereichstitel. Dieser wird als Bezeichner verwendet, nicht als Definition eines benannten Bereichs. |
| startRow | Int32 | Startzeilenindex des Bereichs. |
| startColumn | Int32 | Startspaltenindex des Bereichs. |
| endRow | Int32 | Endzeilenindex des Bereichs. |
| endColumn | Int32 | Endspaltenindex des Bereichs. |

### Rückgabewert

Objektindex.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangeCollectionMethodAddWithStringInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            ProtectedRangeCollection pranges = workbook.Worksheets[0].AllowEditRanges;
            
            // Geschützten Bereich mit Name und Koordinaten hinzufügen
            int index = pranges.Add("Range1", 0, 0, 10, 10);
            
            // Auf den hinzugefügten Bereich zugreifen
            ProtectedRange range = pranges[index];
            
            // Setzen Sie den Sicherheitsdeskriptor fest
            string securityDescriptor = "O:WDG:WDD:(D;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1000)(A;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1013)";
            range.SecurityDescriptor = securityDescriptor;
            
            // Speichern und überprüfen
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [ProtectedRangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


