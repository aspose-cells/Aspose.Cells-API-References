---
title: HorizontalPageBreakCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: HorizontalPageBreakCollection property. Gets the HorizontalPageBreak element at the specified index
type: docs
url: /net/aspose.cells/horizontalpagebreakcollection/item/
---
## HorizontalPageBreakCollection indexer (1 of 2)

Gets the [`HorizontalPageBreak`](../../horizontalpagebreak/) element at the specified index.

```csharp
public HorizontalPageBreak this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add horizontal page breaks
            worksheet.HorizontalPageBreaks.Add(5);
            worksheet.HorizontalPageBreaks.Add(10);
            
            // Access page breaks using Item property
            HorizontalPageBreak firstBreak = worksheet.HorizontalPageBreaks[0];
            Console.WriteLine("First page break row: " + firstBreak.Row);
            
            // Modify cells which affects page breaks
            worksheet.Cells.DeleteRows(0, 2);
            
            // Verify the page break was adjusted
            Console.WriteLine("First page break after row deletion: " + worksheet.HorizontalPageBreaks[0].Row);
        }
    }
}
```

### See Also

* class [HorizontalPageBreak](../../horizontalpagebreak/)
* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HorizontalPageBreakCollection indexer (2 of 2)

Gets the [`HorizontalPageBreak`](../../horizontalpagebreak/) element with the specified cell name.

```csharp
public HorizontalPageBreak this[string cellName] { get; }
```

| Parameter | Description |
| --- | --- |
| cellName | Cell name. |

### Return Value

The element with the specified cell name.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HorizontalPageBreakCollectionPropertyItemDemo2
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add horizontal page breaks
            HorizontalPageBreakCollection hPageBreaks = worksheet.HorizontalPageBreaks;
            int index1 = hPageBreaks.Add(5);
            int index2 = hPageBreaks.Add(15);

            // Access page breaks using Item property
            HorizontalPageBreak break1 = hPageBreaks[index1];
            HorizontalPageBreak break2 = hPageBreaks[index2];

            // Display information about the page breaks
            Console.WriteLine("First page break row: " + break1.Row);
            Console.WriteLine("Second page break row: " + break2.Row);

            // Modify page break by removing the old one and adding a new one
            hPageBreaks.RemoveAt(index1);
            index1 = hPageBreaks.Add(8);
            Console.WriteLine("Modified first page break row: " + hPageBreaks[index1].Row);

            // Remove a page break
            hPageBreaks.RemoveAt(index2);
            Console.WriteLine("Page breaks count after removal: " + hPageBreaks.Count);

            // Save the workbook
            workbook.Save("HorizontalPageBreakCollectionDemo.xlsx");
        }
    }
}
```

### See Also

* class [HorizontalPageBreak](../../horizontalpagebreak/)
* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


