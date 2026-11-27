---
title: "ListObject.RemoveAutoFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObject‑metod. Tar bort auto filter som har tillämpats på denna tabell"
type: docs
url: /sv/net/aspose.cells.tables/listobject/removeautofilter/
---
## ListObject.RemoveAutoFilter method

Tar bort autofilter som är tillämpat på den här tabellen.

```csharp
public void RemoveAutoFilter()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodRemoveAutoFilterDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fyll i exempeldata (med rubrikrad)
            sheet.Cells["A1"].PutValue("ID");
            sheet.Cells["B1"].PutValue("Name");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["B2"].PutValue("Alice");
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["B3"].PutValue("Bob");
            sheet.Cells["A4"].PutValue(3);
            sheet.Cells["B4"].PutValue("Charlie");

            try
            {
                // Lägg till ett ListObject (tabell) som inkluderar ett autofilter som standard
                int listIndex = sheet.ListObjects.Add("A1", "B4", true);
                ListObject listObj = sheet.ListObjects[listIndex];

                // Valfritt: tillämpa ett filter för att demonstrera att ett filter finns
                listObj.Filter();

                // Ta bort autofiltret från ListObject
                listObj.RemoveAutoFilter();

                Console.WriteLine("RemoveAutoFilter called successfully.");
                
                // Spara arbetsboken för att verifiera ändringarna
                workbook.Save("RemoveAutoFilterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during RemoveAutoFilter operation: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


