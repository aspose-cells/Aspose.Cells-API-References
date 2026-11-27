---
title: "WorksheetCollection.Names"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-egenskap. Hämtar samlingen av alla Name-objekt i kalkylarket"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/names/
---
## WorksheetCollection.Names property

Hämtar samlingen av alla Name-objekt i kalkylarket.

```csharp
public NameCollection Names { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyNamesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad med specialtecken i namnet
            Worksheet worksheet = workbook.Worksheets.Add("My.Test");
            
            // Åtkomst till Names-samlingen
            NameCollection names = workbook.Worksheets.Names;
            
            // Lägg till ett nytt namngivet område
            int index = names.Add("My.Test!TestName");
            Name namedRange = names[index];
            
            // Ange områdesreferensen och demonstrera användning
            namedRange.RefersTo = "=My.Test!$A$1:$B$2";
            
            // Skriv ut egenskaperna för det namngivna området
            Console.WriteLine("Name: " + namedRange.Text);
            Console.WriteLine("FullText: " + namedRange.FullText);
            Console.WriteLine("RefersTo: " + namedRange.RefersTo);
        }
    }
}
```

### Se även

* class [NameCollection](../../namecollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


