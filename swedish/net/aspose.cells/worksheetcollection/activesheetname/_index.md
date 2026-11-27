---
title: "WorksheetCollection.ActiveSheetName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-egenskap. Representerar namnet på det aktiva kalkylbladet när kalkylarket öppnas"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/activesheetname/
---
## WorksheetCollection.ActiveSheetName property

Representerar namnet på det aktiva kalkylbladet när kalkylarket öppnas.

```csharp
public string ActiveSheetName { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyActiveSheetNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till några arbetsblad
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Ställ in det aktiva bladet efter namn
            workbook.Worksheets.ActiveSheetName = "Sheet2";

            // Verifiera det aktiva bladet
            Console.WriteLine("Active Sheet: " + workbook.Worksheets.ActiveSheetName);

            // Spara arbetsboken
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


