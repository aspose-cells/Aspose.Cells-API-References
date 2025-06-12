---
title: WorksheetCollection.IsRefreshAllConnections
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection property. Indicates whether refresh all connections on opening file in MS Excel
type: docs
url: /net/aspose.cells/worksheetcollection/isrefreshallconnections/
---
## WorksheetCollection.IsRefreshAllConnections property

Indicates whether refresh all connections on opening file in MS Excel.

```csharp
public bool IsRefreshAllConnections { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyIsRefreshAllConnectionsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the worksheet collection
            WorksheetCollection worksheets = workbook.Worksheets;
            
            // Add some sample worksheets
            worksheets.Add("Sheet1");
            worksheets.Add("Sheet2");
            
            // Set IsRefreshAllConnections property
            worksheets.IsRefreshAllConnections = true;
            
            // Display the current value of IsRefreshAllConnections
            Console.WriteLine("IsRefreshAllConnections: " + worksheets.IsRefreshAllConnections);
            
            // Save the workbook
            workbook.Save("WorksheetCollectionPropertyIsRefreshAllConnectionsDemo.xlsx");
        }
    }
}
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


