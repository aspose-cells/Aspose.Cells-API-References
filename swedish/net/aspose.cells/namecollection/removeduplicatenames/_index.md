---
title: "NameCollection.RemoveDuplicateNames"
second_title: "Aspose.Cells för .NET API‑referens"
description: "NameCollection-metoden. Ta bort de duplicerade definierade namnen"
type: docs
url: /sv/net/aspose.cells/namecollection/removeduplicatenames/
---
## NameCollection.RemoveDuplicateNames method

Ta bort de duplicerade definierade namnen

```csharp
public void RemoveDuplicateNames()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodRemoveDuplicateNamesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till några namngivna områden med duplicerade namn
            worksheet.Cells["A1"].PutValue("Test Value 1");
            worksheet.Cells["B1"].PutValue("Test Value 2");
            
            // Skapa duplicerade namngivna områden med korrekt Add-metodsignatur
            int index1 = workbook.Worksheets.Names.Add("DuplicateName");
            workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$A$1";
            
            int index2 = workbook.Worksheets.Names.Add("DuplicateName");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$B$1";
            
            // Visa antalet innan duplicaten tas bort
            Console.WriteLine($"Named ranges count before removal: {workbook.Worksheets.Names.Count}");
            
            // Ta bort duplicerade namn
            workbook.Worksheets.Names.RemoveDuplicateNames();
            
            // Visa antalet efter att du har tagit bort dubbletter
            Console.WriteLine($"Named ranges count after removal: {workbook.Worksheets.Names.Count}");
        }
    }
}
```

### Se även

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


