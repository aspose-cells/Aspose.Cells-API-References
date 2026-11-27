---
title: "PivotField.OriginalItems"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-egenskap. Hämta de ursprungliga basobjekten"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/originalitems/
---
## PivotField.OriginalItems property

Hämta de ursprungliga basobjekten;

```csharp
public string[] OriginalItems { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyOriginalItemsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑filen
            Workbook workbook = new Workbook("AsposeGroupedField2.xlsx");
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till den första pivottabellen
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Åtkomst till det första radfältet
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Visa ursprungliga objekt och grupperade objekt
            Console.WriteLine("Original Item[0]: " + pivotField.OriginalItems[0]);
            Console.WriteLine("Grouped Item[0]: " + pivotField.Items[0]);
            
            // Spara den modifierade arbetsboken
            workbook.Save("PivotFieldOriginalItemsDemo_Output.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


