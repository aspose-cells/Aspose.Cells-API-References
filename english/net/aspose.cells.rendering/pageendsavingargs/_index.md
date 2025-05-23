---
title: Class PageEndSavingArgs
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Rendering.PageEndSavingArgs class. Info for a page ends saving process
type: docs
url: /net/aspose.cells.rendering/pageendsavingargs/
---
## PageEndSavingArgs class

Info for a page ends saving process.

```csharp
public class PageEndSavingArgs : PageSavingArgs
```

## Properties

| Name | Description |
| --- | --- |
| [HasMorePages](../../aspose.cells.rendering/pageendsavingargs/hasmorepages/) { get; set; } | Gets or sets a value indicating whether having more pages to be output. The default value is true. |
| [PageCount](../../aspose.cells.rendering/pagesavingargs/pagecount/) { get; } | Total page count.(Inherited from [`PageSavingArgs`](../pagesavingargs/).) |
| [PageIndex](../../aspose.cells.rendering/pagesavingargs/pageindex/) { get; } | Current page index, zero based.(Inherited from [`PageSavingArgs`](../pagesavingargs/).) |

### Examples

```csharp
// Called: public void PageEndSaving(PageEndSavingArgs args)
public void Rendering_Type_PageEndSavingArgs(PageEndSavingArgs args)
        {
            Console.WriteLine($"Finished saving page {args.PageIndex}");
        }
```

### See Also

* class [PageSavingArgs](../pagesavingargs/)
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


