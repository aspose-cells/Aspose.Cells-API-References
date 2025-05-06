---
title: Cell.GetValidation
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Gets the validation applied to this cell
type: docs
url: /net/aspose.cells/cell/getvalidation/
---
## Cell.GetValidation method

Gets the validation applied to this cell.

```csharp
public Validation GetValidation()
```

### Examples

```csharp
// Called: res = CompareCollection.Compare(((object[])cells[&amp;quot;D3&amp;quot;].GetValidation().Value1).GetEnumerator(),
[Test]
       public void Method_GetValidation()
       {
           Workbook workbook = new Workbook(Constants.sourcePath + &quot;Validation/N44505_738775.xlsx&quot;);
           Cells cells = workbook.Worksheets[0].Cells;
           ICollectionItemComparator comparator = new ItemComparatorOfCommonObject();
           string res;
           
           // Dispaly the first drop-down&apos;s values:
           res = CompareCollection.Compare(((object[])cells[&quot;B1&quot;].GetValidation().Value1).GetEnumerator(),
               new object[] { &quot;Pizza&quot;, &quot;IHOP&quot;, &quot;Chinese&quot; }, comparator);
           if (res != null)
           {
               AssertHelper.Fail(&quot;B1.Validation.Value1: &quot; + res);
           }

           // Set the drop-down value...
           cells[&quot;B1&quot;].Value = &quot;IHOP&quot;;

           // Now display the second drop-down values list (it uses INDIRECT/Ranges)
           res = CompareCollection.Compare(((object[])cells[&quot;D1&quot;].GetValidation().Value1).GetEnumerator(),
               new object[] { &quot;Pancakces&quot;, &quot;Combos&quot;, &quot;French_Toast&quot;, &quot;Waffles&quot;, }, comparator);
           if (res != null)
           {
               AssertHelper.Fail(&quot;D1.Validation.Value1: &quot; + res);
           }

           // Now disply what the list *should* be, just using the range directly.
           res = CompareCollection.Compare(((object[])cells[&quot;D3&quot;].GetValidation().Value1).GetEnumerator(),
               new object[] { &quot;Pancakces&quot;, &quot;Combos&quot;, &quot;French_Toast&quot;, &quot;Waffles&quot; }, comparator);
           if (res != null)
           {
               AssertHelper.Fail(&quot;D3.Validation.Value1: &quot; + res);
           }
       }
```

### See Also

* class [Validation](../../validation/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


