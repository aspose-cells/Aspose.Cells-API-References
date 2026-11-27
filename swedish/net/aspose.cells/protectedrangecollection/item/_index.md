---
title: "ProtectedRangeCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ProtectedRangeCollection-egenskap. Hämtar ProtectedRange-elementet vid det angivna indexet"
type: docs
url: /sv/net/aspose.cells/protectedrangecollection/item/
---
## ProtectedRangeCollection indexer

Hämtar [`ProtectedRange`](../../protectedrange/) elementet vid det angivna indexet.

```csharp
public ProtectedRange this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Det nollbaserade indexet för elementet. |

### Returvärde

Elementet på det angivna indexet.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangeCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till ett skyddat område med cellindex (startRow, startColumn, endRow, endColumn)
            int index = worksheet.AllowEditRanges.Add("MyProtectedRange", 0, 0, 1, 1);
            ProtectedRange protectedRange = worksheet.AllowEditRanges[index];
            protectedRange.Password = "password123";
            
            // Åtkomst till det skyddade området med Item-egenskapen (index 0)
            ProtectedRange retrievedRange = worksheet.AllowEditRanges[0];
            
            // Verifiera och visa skyddstatus
            Console.WriteLine("Is protected with password: " + retrievedRange.IsProtectedWithPassword);
            Console.WriteLine("Range name: " + retrievedRange.Name);
            
            // Spara arbetsboken
            workbook.Save("ProtectedRangeDemo.xlsx");
        }
    }
}
```

### Se även

* class [ProtectedRange](../../protectedrange/)
* class [ProtectedRangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


