---
title: DataSorter.Order2
second_title: Aspose.Cells for .NET API Reference
description: DataSorter property. Represents sort order of the second key
type: docs
url: /net/aspose.cells/datasorter/order2/
---
## DataSorter.Order2 property

Represents sort order of the second key.

```csharp
public SortOrder Order2 { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(dsorterSrc.Order2, dsortDest.Order2, info + ".Order2");
public static void Property_Order2(DataSorter dsorterSrc, DataSorter dsortDest, string info)
        {
            if (AssertHelper.checkNull(dsorterSrc, dsortDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(dsorterSrc.CaseSensitive, dsortDest.CaseSensitive, info + ".CaseSensitive");
            AssertHelper.AreEqual(dsorterSrc.HasHeaders, dsortDest.HasHeaders, info + ".HasHeaders");
            AssertHelper.AreEqual(dsorterSrc.Key1, dsortDest.Key1, info + ".Key1");
            AssertHelper.AreEqual(dsorterSrc.Key2, dsortDest.Key2, info + ".Key2");
            AssertHelper.AreEqual(dsorterSrc.Key3, dsortDest.Key3, info + ".Key3");
            AssertHelper.AreEqual(dsorterSrc.Order1, dsortDest.Order1, info + ".Order1");
            AssertHelper.AreEqual(dsorterSrc.Order2, dsortDest.Order2, info + ".Order2");
            AssertHelper.AreEqual(dsorterSrc.Order3, dsortDest.Order3, info + ".Order3");
            AssertHelper.AreEqual(dsorterSrc.SortLeftToRight, dsortDest.SortLeftToRight, info + ".SortLeftToRight");
        }
```

### See Also

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


