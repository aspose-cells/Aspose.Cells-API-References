---
title: "WorksheetCollection.TableStyles"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-egenskap. Hämtar TableStyles-objektet"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/tablestyles/
---
## WorksheetCollection.TableStyles property

Hämtar `TableStyles`-objektet.

```csharp
public TableStyleCollection TableStyles { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyTableStylesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till några arbetsblad
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            
            // Skapa och lägg till tabellstilar
            int styleIndex1 = workbook.Worksheets.TableStyles.AddTableStyle("Style1");
            TableStyle style1 = workbook.Worksheets.TableStyles[styleIndex1];
            
            int styleIndex2 = workbook.Worksheets.TableStyles.AddTableStyle("Style2");
            TableStyle style2 = workbook.Worksheets.TableStyles[styleIndex2];
            
            // Visa antalet tabellstilar
            Console.WriteLine("Table styles count: " + workbook.Worksheets.TableStyles.Count);
            
            // Ta bort en stil
            workbook.Worksheets.TableStyles.RemoveAt(0);
            
            // Visa uppdaterat antal
            Console.WriteLine("Table styles count after removal: " + workbook.Worksheets.TableStyles.Count);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [TableStyleCollection](../../../aspose.cells.tables/tablestylecollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


