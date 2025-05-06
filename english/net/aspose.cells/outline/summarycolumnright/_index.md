---
title: Outline.SummaryColumnRight
second_title: Aspose.Cells for .NET API Reference
description: Outline property. Indicates if the summary column will be positioned to the right of the detail columns in the outline
type: docs
url: /net/aspose.cells/outline/summarycolumnright/
---
## Outline.SummaryColumnRight property

Indicates if the summary column will be positioned to the right of the detail columns in the outline.

```csharp
public bool SummaryColumnRight { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(outlineSrc.SummaryColumnRight, outlineDest.SummaryColumnRight, info + &amp;quot;.SummaryColumnRight&amp;quot;);
public static void Property_SummaryColumnRight(Outline outlineSrc, Outline outlineDest, string info)
        {
            if (AssertHelper.checkNull(outlineSrc, outlineDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(outlineSrc.SummaryColumnRight, outlineDest.SummaryColumnRight, info + &quot;.SummaryColumnRight&quot;);
            AssertHelper.AreEqual(outlineSrc.SummaryRowBelow, outlineDest.SummaryRowBelow, info + &quot;.SummaryRowBelow&quot;);
        }
```

### See Also

* class [Outline](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


