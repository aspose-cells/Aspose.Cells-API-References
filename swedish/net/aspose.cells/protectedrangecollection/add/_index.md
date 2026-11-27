---
title: "ProtectedRangeCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ProtectedRangeCollection‑metod. Lägger till ett ProtectedRange‑objekt i samlingen"
type: docs
url: /sv/net/aspose.cells/protectedrangecollection/add/
---
## ProtectedRangeCollection.Add method

Lägger till ett [`ProtectedRange`](../../protectedrange/)‑objekt i samlingen.

```csharp
public int Add(string name, int startRow, int startColumn, int endRow, int endColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | Områdestitel. Detta används som en beskrivning, inte som en namngiven områdesdefinition. |
| startRow | Int32 | Startradens index för området. |
| startColumn | Int32 | Startkolumnens index för intervallet. |
| endRow | Int32 | Slutradens index för intervallet. |
| endColumn | Int32 | Slutkolumnens index för intervallet. |

### Returvärde

objektindex.

### Exempel

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
            
            // Lägg till skyddat område med namn och koordinater
            int index = pranges.Add("Range1", 0, 0, 10, 10);
            
            // Åtkomst till det tillagda området.
            ProtectedRange range = pranges[index];
            
            // Ställ in säkerhetsbeskrivning
            string securityDescriptor = "O:WDG:WDD:(D;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1000)(A;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1013)";
            range.SecurityDescriptor = securityDescriptor;
            
            // Spara och verifiera
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [ProtectedRangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


