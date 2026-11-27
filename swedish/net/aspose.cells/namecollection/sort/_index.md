---
title: "NameCollection.Sort"
second_title: "Aspose.Cells för .NET API‑referens"
description: "NameCollection-metoden. Sorterar definierade namn"
type: docs
url: /sv/net/aspose.cells/namecollection/sort/
---
## NameCollection.Sort method

Sorterar definierade namn.

```csharp
public void Sort()
```

### Anmärkningar

Om du skapar ett stort antal namngivna områden i Excel-filen, vänligen anropa den här metoden efter att alla namngivna områden har skapats och innan du sparar

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameCollectionMethodSortDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hämta NameCollection från arbetsboken
            NameCollection names = workbook.Worksheets.Names;
            
            // Lägg till några namngivna områden för att demonstrera sortering
            names.Add("RangeC");
            names.Add("RangeA");
            names.Add("RangeB");
            
            try
            {
                // Visa namn före sortering
                Console.WriteLine("Names before sorting:");
                foreach (Name name in names)
                {
                    Console.WriteLine(name.Text);
                }
                
                // Anropa Sort-metoden
                names.Sort();
                
                // Visa namn efter sortering
                Console.WriteLine("\nNames after sorting:");
                foreach (Name name in names)
                {
                    Console.WriteLine(name.Text);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Sort method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("NameCollectionSortDemo.xlsx");
        }
    }
}
```

### Se även

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


