---
title: RangeCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: RangeCollection method. Adds a Range item to the collection
type: docs
url: /net/aspose.cells/rangecollection/add/
---
## RangeCollection.Add method

Adds a [`Range`](../../range/) item to the collection.

```csharp
[Obsolete("Use RangeCollection.AddRange(Range) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(Range range)
```

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | Range object |

### Remarks

NOTE: This member is now obsolete. Instead, please use AddRange() method. This method will be removed 6 months later since December 2025. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeCollectionMethodAddWithRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Create a range and add it to the collection
            Aspose.Cells.Range cellRange = worksheet.Cells.CreateRange(0, 0, 3, 1);
            worksheet.Cells.Ranges.Add(cellRange);
            
            // Insert rows to demonstrate the range expands
            worksheet.Cells.InsertRows(2, 2);
            
            Console.WriteLine("Range row count after insertion: " + cellRange.RowCount);
        }
    }
}
```

### See Also

* class [Range](../../range/)
* class [RangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


