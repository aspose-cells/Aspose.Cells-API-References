---
title: "NameCollection.RemoveAt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "NameCollection-metoden. Ta bort namnet på det specifika indexet"
type: docs
url: /sv/net/aspose.cells/namecollection/removeat/
---
## NameCollection.RemoveAt method

Ta bort namnet på det specifika indexet.

```csharp
public void RemoveAt(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | index för namnet som ska tas bort. |

### Anmärkningar

Se till att namnet inte refereras av andra formler innan du anropar metoden. Och om namnet refereras, är det bättre att sätta Name.RefersTo till null.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WorksheetCollection worksheets = workbook.Worksheets;
            NameCollection names = worksheets.Names;

            // Lägg till namn i samlingen
            int firstIndex = names.Add("FirstRange");
            names[firstIndex].RefersTo = "=Sheet1!$A$1:$A$5";
            
            int secondIndex = names.Add("SecondRange");
            names[secondIndex].RefersTo = "=Sheet1!$B$1:$B$5";

            // Ta bort namn efter index
            names.RemoveAt(firstIndex);

            // Verifiera borttagning genom att kontrollera antalet
            Console.WriteLine($"Remaining names count: {names.Count}");

            workbook.Save("NameCollectionRemoveAtExample.xlsx");
        }
    }
}
```

### Se även

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


