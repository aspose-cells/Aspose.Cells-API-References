---
title: "Name.RefersTo"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Name-egenskap. Returnerar eller anger formeln som namnet är definierat att referera till, inledande med ett likhetstecken"
type: docs
url: /sv/net/aspose.cells/name/refersto/
---
## Name.RefersTo property

Returnerar eller anger formeln som namnet är definierat att referera till, inledningsvis med ett likhetstecken.

```csharp
public string RefersTo { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyRefersToDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "Sheet1";

            // Lägg till namngivna områden med RefersTo
            int index1 = workbook.Worksheets.Names.Add("NamedRange1");
            workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$6:$8";
            
            int index2 = workbook.Worksheets.Names.Add("NamedRange2");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$C:$D";

            // Visa RefersTo-egenskapen för namngivna områden
            Console.WriteLine("NamedRange1 RefersTo: " + workbook.Worksheets.Names[0].RefersTo);
            Console.WriteLine("NamedRange2 RefersTo: " + workbook.Worksheets.Names[1].RefersTo);
        }
    }
}
```

### Se även

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


