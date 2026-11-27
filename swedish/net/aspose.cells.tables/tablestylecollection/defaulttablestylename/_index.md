---
title: "TableStyleCollection.DefaultTableStyleName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TableStyleCollection-egenskap. Hämtar och anger standardstilnamnet för tabellen"
type: docs
url: /sv/net/aspose.cells.tables/tablestylecollection/defaulttablestylename/
---
## TableStyleCollection.DefaultTableStyleName property

Hämtar och anger standardstilnamnet för tabellen.

```csharp
public string DefaultTableStyleName { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleCollectionPropertyDefaultTableStyleNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Få åtkomst till samlingen av tabellstilar
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            
            // Visa standardtabellstilens namn
            Console.WriteLine("Default Table Style: " + tableStyles.DefaultTableStyleName);
            
            // Ändra standardtabellstilen
            tableStyles.DefaultTableStyleName = "TableStyleMedium9";
            Console.WriteLine("New Default Table Style: " + tableStyles.DefaultTableStyleName);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


