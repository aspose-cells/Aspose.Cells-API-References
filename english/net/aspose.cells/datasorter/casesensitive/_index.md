---
title: DataSorter.CaseSensitive
second_title: Aspose.Cells for .NET API Reference
description: DataSorter property. Gets and sets whether case sensitive when comparing string
type: docs
url: /net/aspose.cells/datasorter/casesensitive/
---
## DataSorter.CaseSensitive property

Gets and sets whether case sensitive when comparing string.

```csharp
public bool CaseSensitive { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(dsorterSrc.CaseSensitive, dsortDest.CaseSensitive, info + &amp;quot;.CaseSensitive&amp;quot;);
public static void Property_CaseSensitive(DataSorter dsorterSrc, DataSorter dsortDest, string info)
        {
            if (AssertHelper.checkNull(dsorterSrc, dsortDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(dsorterSrc.CaseSensitive, dsortDest.CaseSensitive, info + &quot;.CaseSensitive&quot;);
            AssertHelper.AreEqual(dsorterSrc.HasHeaders, dsortDest.HasHeaders, info + &quot;.HasHeaders&quot;);
            AssertHelper.AreEqual(dsorterSrc.Key1, dsortDest.Key1, info + &quot;.Key1&quot;);
            AssertHelper.AreEqual(dsorterSrc.Key2, dsortDest.Key2, info + &quot;.Key2&quot;);
            AssertHelper.AreEqual(dsorterSrc.Key3, dsortDest.Key3, info + &quot;.Key3&quot;);
            AssertHelper.AreEqual(dsorterSrc.Order1, dsortDest.Order1, info + &quot;.Order1&quot;);
            AssertHelper.AreEqual(dsorterSrc.Order2, dsortDest.Order2, info + &quot;.Order2&quot;);
            AssertHelper.AreEqual(dsorterSrc.Order3, dsortDest.Order3, info + &quot;.Order3&quot;);
            AssertHelper.AreEqual(dsorterSrc.SortLeftToRight, dsortDest.SortLeftToRight, info + &quot;.SortLeftToRight&quot;);
        }
```

### See Also

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


