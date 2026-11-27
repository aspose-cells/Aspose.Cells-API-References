---
title: "TableStyleCollection.DefaultPivotStyleName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TableStyleCollection-egenskap. Hämtar och anger standardstilnamnet för pivottabellen"
type: docs
url: /sv/net/aspose.cells.tables/tablestylecollection/defaultpivotstylename/
---
## TableStyleCollection.DefaultPivotStyleName property

Hämtar och anger standardstilnamnet för pivottabellen.

```csharp
public string DefaultPivotStyleName { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleCollectionPropertyDefaultPivotStyleNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Få åtkomst till samlingen av tabellstilar
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            
            // Visa standardstilnamnet för pivottabellen
            Console.WriteLine("Default Pivot Style: " + tableStyles.DefaultPivotStyleName);
            
            // Ändra standardstilen för pivottabellen
            tableStyles.DefaultPivotStyleName = "PivotStyleDark2";
            
            // Verifiera ändringen
            Console.WriteLine("Updated Default Pivot Style: " + tableStyles.DefaultPivotStyleName);
            
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


