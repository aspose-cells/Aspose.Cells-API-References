---
title: Class PageStartSavingArgs
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Rendering.PageStartSavingArgs class. Info for a page starts saving process
type: docs
url: /net/aspose.cells.rendering/pagestartsavingargs/
---
## PageStartSavingArgs class

Info for a page starts saving process.

```csharp
public class PageStartSavingArgs : PageSavingArgs
```

## Properties

| Name | Description |
| --- | --- |
| [IsToOutput](../../aspose.cells.rendering/pagestartsavingargs/istooutput/) { get; set; } | Gets or sets a value indicating whether the page should be output. The default value is true. |
| [PageCount](../../aspose.cells.rendering/pagesavingargs/pagecount/) { get; } | Total page count.(Inherited from [`PageSavingArgs`](../pagesavingargs/).) |
| [PageIndex](../../aspose.cells.rendering/pagesavingargs/pageindex/) { get; } | Current page index, zero based.(Inherited from [`PageSavingArgs`](../pagesavingargs/).) |

### Examples

```csharp
// Called: public void PageStartSaving(PageStartSavingArgs args)
public void Type_PageStartSavingArgs(PageStartSavingArgs args)
        {
            Console.WriteLine($"Starting to save page {args.PageIndex}");
        }
```

### See Also

* class [PageSavingArgs](../pagesavingargs/)
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


