---
title: "Workbook.Worksheets"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-egenskap. Hämtar WorksheetCollection‑samlingen i kalkylbladet"
type: docs
url: /sv/net/aspose.cells/workbook/worksheets/
---
## Workbook.Worksheets property

Hämtar [`WorksheetCollection`](../../worksheetcollection/)‑samlingen i kalkylbladet.

```csharp
public WorksheetCollection Worksheets { get; }
```

### Returvärde

[`WorksheetCollection`](../../worksheetcollection/) collection

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyWorksheetsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            
            // Lägg till ett nytt arbetsblad
            workbook.Worksheets.Add("SecondSheet");
            
            // Åtkomst till det andra kalkylbladet och lägg till data
            Worksheet secondSheet = workbook.Worksheets[1];
            secondSheet.Cells["A1"].PutValue("Product");
            secondSheet.Cells["B1"].PutValue("Price");
            secondSheet.Cells["A2"].PutValue("Laptop");
            secondSheet.Cells["B2"].PutValue(999.99);
            
            // Spara arbetsboken
            workbook.Save("WorkbookWorksheetsDemo.xlsx");
            
            // Skriv ut antalet kalkylblad
            Console.WriteLine($"Number of worksheets: {workbook.Worksheets.Count}");
        }
    }
}
```

### Se även

* class [WorksheetCollection](../../worksheetcollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


