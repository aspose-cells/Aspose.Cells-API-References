---
title: "AutoFilter.FilterColumns"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFilter-egenskap. Hämtar samlingen av filterkolumnerna"
type: docs
url: /sv/net/aspose.cells/autofilter/filtercolumns/
---
## AutoFilter.FilterColumns property

Hämtar samlingen av filterkolumnerna.

```csharp
public FilterColumnCollection FilterColumns { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertyFilterColumnsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Department");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["C1"].PutValue("Status");
            
            worksheet.Cells["A2"].PutValue("HR");
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["C2"].PutValue("Present");
            
            worksheet.Cells["A3"].PutValue("IT");
            worksheet.Cells["B3"].PutValue("Sarah");
            worksheet.Cells["C3"].PutValue("Absent");
            
            worksheet.Cells["A4"].PutValue("HR");
            worksheet.Cells["B4"].PutValue("Mike");
            worksheet.Cells["C4"].PutValue("Present");

            // Applicera autofilter
            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.Range = "A1:C1";
            
            // Filtrera kolumn 2 (Status) för "Present"-värden
            autoFilter.Filter(2, "Present");
            
            // Åtkomst till filterkolumnen
            FilterColumn filterColumn = autoFilter.FilterColumns[2];
            
            // Spara arbetsboken
            workbook.Save("AutoFilterExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [FilterColumnCollection](../../filtercolumncollection/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


