---
title: ListObject.ShowTotals
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets and sets whether this ListObject show total row
type: docs
url: /net/aspose.cells.tables/listobject/showtotals/
---
## ListObject.ShowTotals property

Gets and sets whether this ListObject show total row.

```csharp
public bool ShowTotals { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(loSrc.ShowTotals, loDest.ShowTotals, info + ".ShowTotals");
public static void Property_ShowTotals(ListObject loSrc, ListObject loDest, string info)
        {
            if (AssertHelper.checkNull(loSrc, loDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(loSrc.StartRow, loDest.StartRow, info + ".StartRow");
            AssertHelper.AreEqual(loSrc.EndRow, loDest.EndRow, info + ".EndRow");
            AssertHelper.AreEqual(loSrc.StartColumn, loDest.StartColumn, info + ".StartColumn");
            AssertHelper.AreEqual(loSrc.EndColumn, loDest.EndColumn, info + ".EndColumn");
            RangesTest.Property_ShowTotals(loSrc.DataRange, loDest.DataRange, info + ".DataRange");    
            ListColumnsTest.Property_ShowTotals(loSrc.ListColumns, loDest.ListColumns, info + ".ListColumns");
            AssertHelper.AreEqual(loSrc.ShowTotals, loDest.ShowTotals, info + ".ShowTotals");        
        }
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


