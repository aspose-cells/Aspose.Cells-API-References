---
title: ListObject.EndColumn
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets the end column of the range
type: docs
url: /net/aspose.cells.tables/listobject/endcolumn/
---
## ListObject.EndColumn property

Gets the end column of the range.

```csharp
public int EndColumn { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(loSrc.EndColumn, loDest.EndColumn, info + &amp;quot;.EndColumn&amp;quot;);
public static void Property_EndColumn(ListObject loSrc, ListObject loDest, string info)
        {
            if (AssertHelper.checkNull(loSrc, loDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(loSrc.StartRow, loDest.StartRow, info + &quot;.StartRow&quot;);
            AssertHelper.AreEqual(loSrc.EndRow, loDest.EndRow, info + &quot;.EndRow&quot;);
            AssertHelper.AreEqual(loSrc.StartColumn, loDest.StartColumn, info + &quot;.StartColumn&quot;);
            AssertHelper.AreEqual(loSrc.EndColumn, loDest.EndColumn, info + &quot;.EndColumn&quot;);
            RangesTest.Property_EndColumn(loSrc.DataRange, loDest.DataRange, info + &quot;.DataRange&quot;);    
            ListColumnsTest.Property_EndColumn(loSrc.ListColumns, loDest.ListColumns, info + &quot;.ListColumns&quot;);
            AssertHelper.AreEqual(loSrc.ShowTotals, loDest.ShowTotals, info + &quot;.ShowTotals&quot;);        
        }
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


