---
title: "Name.FullText"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Name-egenskap. Hämtar namnens fulla text för objektet med omfångsinställningen"
type: docs
url: /sv/net/aspose.cells/name/fulltext/
---
## Name.FullText property

Hämtar namnets fullständiga text för objektet med omfångsinställningen.

```csharp
public string FullText { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyFullTextDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa några namngivna områden
            worksheet.Cells["A1"].PutValue("Test Value");
            worksheet.Cells.CreateRange("A1", "B5").Name = "TestRange1";
            worksheet.Cells.CreateRange("C1", "D5").Name = "TestRange2";
            
            // Hämta namnkollektionen
            NameCollection names = workbook.Worksheets.Names;
            
            // Hitta ett namn med dess FullText
            string reference = "=Sheet1!$A$1:$B$5";
            Name foundName = FindNameByFullText(names, reference);
            
            // Skriv ut resultat
            if (foundName != null)
            {
                Console.WriteLine("Found name: " + foundName.Text);
                Console.WriteLine("FullText: " + foundName.FullText);
            }
            else
            {
                Console.WriteLine("Name not found");
            }
        }
        
        public static Name FindNameByFullText(NameCollection names, string reference)
        {
            if (reference.IndexOf('=') == 0)
            {
                reference = reference.Substring(1);
            }
            foreach (Name nm in names)
            {
                if (nm.FullText.Equals(reference))
                {
                    return nm;
                }
            }
            return null;
        }
    }
}
```

### Se även

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


