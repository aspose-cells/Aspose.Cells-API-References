---
title: "Workbook.RemovePersonalInformation"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Tar bort personlig information"
type: docs
url: /sv/net/aspose.cells/workbook/removepersonalinformation/
---
## Workbook.RemovePersonalInformation method

Tar bort personlig information.

```csharp
public void RemovePersonalInformation()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemovePersonalInformationDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Lägg till en kommentar med författarinformation
            int commentIndex = sheet.Comments.Add("A1");
            sheet.Comments[commentIndex].Note = "Sample comment";
            sheet.Comments[commentIndex].Author = "Test Author";
            
            // Visa original författarinformation
            Console.WriteLine("Before removal - Comment Author: " + sheet.Comments[commentIndex].Author);
            
            // Ta bort personlig information
            wb.RemovePersonalInformation();
            
            // Spara arbetsboken
            wb.Save("output.xlsx", SaveFormat.Xlsx);
            
            // Läs in igen för att verifiera borttagning
            Workbook wb2 = new Workbook("output.xlsx");
            Console.WriteLine("After removal - Comment Author: " + wb2.Worksheets[0].Comments[commentIndex].Author);
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


