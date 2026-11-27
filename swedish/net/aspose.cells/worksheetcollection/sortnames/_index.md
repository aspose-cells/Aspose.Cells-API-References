---
title: "WorksheetCollection.SortNames"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-metoden. Sorterar de definierade namnen"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/sortnames/
---
## WorksheetCollection.SortNames method

Sorterar de definierade namnen.

```csharp
public void SortNames()
```

### Anmärkningar

Om du skapar ett stort antal namngivna områden i Excel-filen, vänligen anropa den här metoden efter att alla namngivna områden har skapats och innan du sparar

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodSortNamesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till några namngivna områden
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test1");
            worksheet.Cells.CreateRange("A1").Name = "Range2";
            worksheet.Cells["B1"].PutValue("Test2");
            worksheet.Cells.CreateRange("B1").Name = "Range1";
            
            // Visa namn före sortering
            Console.WriteLine("Before sorting:");
            foreach (Name name in workbook.Worksheets.Names)
            {
                Console.WriteLine(name.RefersTo);
            }
            
            // Sortera namnen
            workbook.Worksheets.SortNames();
            
            // Visa namn efter sortering
            Console.WriteLine("\nAfter sorting:");
            foreach (Name name in workbook.Worksheets.Names)
            {
                Console.WriteLine(name.RefersTo);
            }
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


