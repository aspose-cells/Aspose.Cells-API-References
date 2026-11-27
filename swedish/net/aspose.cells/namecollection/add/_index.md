---
title: "NameCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "NameCollection-metoden. Definierar ett nytt namn"
type: docs
url: /sv/net/aspose.cells/namecollection/add/
---
## NameCollection.Add method

Definierar ett nytt namn.

```csharp
public int Add(string text)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| text | String | Texten att använda som namn. |

### Returvärde

[`Name`](../../name/) object index.

### Anmärkningar

Namnet får inte innehålla mellanslag och får inte se ut som cellreferenser.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook(FileFormatType.Xlsx);
            Worksheet worksheet = wb.Worksheets[0];
            
            // Lägg till ett namn med strängreferens
            int index = wb.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = wb.Worksheets.Names[index];
            
            // Ange formeln som namnet refererar till
            namedRange.RefersTo = "=Sheet1!$A$1:$B$10";
            
            // Verifiera och skriv ut resultaten
            Console.WriteLine("Named Range RefersTo: " + namedRange.RefersTo);
            Console.WriteLine("Named Range Index: " + index);
            
            // Hämta området och visa dess adress
            Aspose.Cells.Range range = namedRange.GetRange();
            Console.WriteLine("Range Address: " + range.Address);
        }
    }
}
```

### Se även

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


