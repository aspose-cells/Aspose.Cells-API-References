---
title: DataSorter.Key2
second_title: Aspose.Cells for .NET API Reference
description: DataSorter property. Represents second sorted column indexabsolute position column A is 0 B is 1 
type: docs
url: /net/aspose.cells/datasorter/key2/
---
## DataSorter.Key2 property

Represents second sorted column index(absolute position, column A is 0, B is 1, ...).

```csharp
public int Key2 { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(dsorterSrc.Key2, dsortDest.Key2, info + ".Key2");
public static void DataSorter_Property_Key2(DataSorter dsorterSrc, DataSorter dsortDest, string info)
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

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


