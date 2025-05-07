---
title: Outline.SummaryRowBelow
second_title: Aspose.Cells for .NET API Reference
description: Outline property. Indicates if the summary row will be positioned below the detail rows in the outline
type: docs
url: /net/aspose.cells/outline/summaryrowbelow/
---
## Outline.SummaryRowBelow property

Indicates if the summary row will be positioned below the detail rows in the outline.

```csharp
public bool SummaryRowBelow { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(outlineSrc.SummaryRowBelow, outlineDest.SummaryRowBelow, info + ".SummaryRowBelow");
public static void Property_SummaryRowBelow(Outline outlineSrc, Outline outlineDest, string info)
        {
            if (AssertHelper.checkNull(outlineSrc, outlineDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(outlineSrc.SummaryColumnRight, outlineDest.SummaryColumnRight, info + ".SummaryColumnRight");
            AssertHelper.AreEqual(outlineSrc.SummaryRowBelow, outlineDest.SummaryRowBelow, info + ".SummaryRowBelow");
        }
```

### See Also

* class [Outline](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


