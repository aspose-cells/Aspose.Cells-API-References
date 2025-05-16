---
title: VerticalPageBreakCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: VerticalPageBreakCollection property. Gets the VerticalPageBreak element at the specified index
type: docs
url: /net/aspose.cells/verticalpagebreakcollection/item/
---
## VerticalPageBreakCollection indexer (1 of 2)

Gets the [`VerticalPageBreak`](../../verticalpagebreak/) element at the specified index.

```csharp
public VerticalPageBreak this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: AssertHelper.AreEqual(vpagebreaksSrc[i], vpagebreaksDest[i], info + ".VPageBreak");
public static void VerticalPageBreakCollection_Property_Item(VerticalPageBreakCollection vpagebreaksSrc, VerticalPageBreakCollection vpagebreaksDest, string info)
        {
            if (AssertHelper.checkNull(vpagebreaksSrc, vpagebreaksDest, info))
            {
                return;
            }
            int countSrc = vpagebreaksSrc.Count;
            int countDest = vpagebreaksDest.Count;
            AssertHelper.AreEqual(countSrc, countDest, info + ".Count");
            for (int i = 0; i < countSrc && i < countDest; i++)
            {
                AssertHelper.AreEqual(vpagebreaksSrc[i], vpagebreaksDest[i], info + ".VPageBreak");
            }
        }
```

### See Also

* class [VerticalPageBreak](../../verticalpagebreak/)
* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## VerticalPageBreakCollection indexer (2 of 2)

Gets the [`VerticalPageBreak`](../../verticalpagebreak/) element with the specified cell name.

```csharp
public VerticalPageBreak this[string cellName] { get; }
```

| Parameter | Description |
| --- | --- |
| cellName | Cell name. |

### Return Value

The element with the specified cell name.

### Examples

```csharp
namespace AsposeCellsExamples.VerticalPageBreakCollectionPropertyItemDemo
{
    using Aspose.Cells;
    using System;

    public class VerticalPageBreakCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some vertical page breaks
            VerticalPageBreakCollection vPageBreaks = worksheet.VerticalPageBreaks;
            int index1 = vPageBreaks.Add(5);
            int index2 = vPageBreaks.Add(10);
            int index3 = vPageBreaks.Add(15);

            // Access page breaks using Item property by index
            VerticalPageBreak break1 = vPageBreaks[index1];
            VerticalPageBreak break2 = vPageBreaks[index2];
            VerticalPageBreak break3 = vPageBreaks[index3];

            // Display column numbers of the page breaks
            Console.WriteLine("Page break 1 column: " + break1.Column);
            Console.WriteLine("Page break 2 column: " + break2.Column);
            Console.WriteLine("Page break 3 column: " + break3.Column);

            // Modify the worksheet to show effect of page breaks
            for (int i = 0; i < 20; i++)
            {
                worksheet.Cells[0, i].Value = "Column " + i;
            }

            // Save the workbook with page breaks
            workbook.Save("VerticalPageBreakCollectionItemDemo.xlsx");
        }
    }
}
```

### See Also

* class [VerticalPageBreak](../../verticalpagebreak/)
* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


