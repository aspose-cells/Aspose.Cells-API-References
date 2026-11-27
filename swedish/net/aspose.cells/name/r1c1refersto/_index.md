---
title: "Name.R1C1RefersTo"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Name-egenskap. Hämtar eller anger en R1C1-referens för Name"
type: docs
url: /sv/net/aspose.cells/name/r1c1refersto/
---
## Name.R1C1RefersTo property

Hämtar eller anger en R1C1-referens för [`Name`](../).

```csharp
public string R1C1RefersTo { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyR1C1RefersToDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett nytt namn i namnkollektionen
            int nameIndex = workbook.Worksheets.Names.Add("TestRange");
            Name name = workbook.Worksheets.Names[nameIndex];
            
            // Ange R1C1-referens för namnet
            name.R1C1RefersTo = "'Sheet1'!R3C1:R9C4";
            
            // Verifiera att referensen har satts korrekt
            Console.WriteLine("Name refers to: " + name.RefersTo);
            
            // Spara arbetsboken
            workbook.Save("NamePropertyR1C1RefersToDemo_Output.xlsx");
        }
    }
}
```

### Se även

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


