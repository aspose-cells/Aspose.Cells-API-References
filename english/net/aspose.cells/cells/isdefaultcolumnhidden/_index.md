---
title: Cells.IsDefaultColumnHidden
second_title: Aspose.Cells for .NET API Reference
description: Cells property. 
type: docs
url: /net/aspose.cells/cells/isdefaultcolumnhidden/
---
## Cells.IsDefaultColumnHidden property

```csharp
public bool IsDefaultColumnHidden { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyIsDefaultColumnHiddenDemo
    {
        public static void Run()
        {
            try
            {
                // Create a new workbook and get the first worksheet
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                Cells cells = worksheet.Cells;

                // Add some data so the worksheet is not empty
                cells["A1"].PutValue("First");
                cells["B1"].PutValue("Second");
                cells["C1"].PutValue("Third");

                // Read the IsDefaultColumnHidden property (default is false)
                bool isDefaultColumnHidden = cells.IsDefaultColumnHidden;
                Console.WriteLine("IsDefaultColumnHidden: " + isDefaultColumnHidden);

                // Save the workbook (optional, just to complete the demo)
                workbook.Save("IsDefaultColumnHiddenDemo.xlsx", SaveFormat.Xlsx);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


