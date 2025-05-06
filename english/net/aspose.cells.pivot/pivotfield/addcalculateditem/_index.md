---
title: PivotField.AddCalculatedItem
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Add a calculated formula item to the pivot field
type: docs
url: /net/aspose.cells.pivot/pivotfield/addcalculateditem/
---
## PivotField.AddCalculatedItem method

Add a calculated formula item to the pivot field.

```csharp
public void AddCalculatedItem(string name, string formula)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The item's name. |
| formula | String | The formula of pivot item. |

### Remarks

Only supports to add calculated item to Row/Column field.

### Examples

```csharp
// Called: pivotTable.RowFields[0].AddCalculatedItem(&amp;quot;Test&amp;quot;, &amp;quot;=&amp;apos;1&amp;apos;&amp;quot;);
[Test]
        public void Method_String_()
        {
            var wb = new Workbook(Constants.openPivottablePath + &quot;Dummy2.xlsx&quot;);
            Aspose.Cells.Pivot.PivotTable pivotTable = wb.Worksheets[1].PivotTables[0];
            pivotTable.RowFields[0].AddCalculatedItem(&quot;Test&quot;, &quot;=&apos;1&apos;&quot;);
            wb.Save(Constants.savePivottablePath + &quot;29408.xlsx&quot;);


            wb = new Workbook(Constants.openPivottablePath + &quot;R.xls&quot;);
            pivotTable = wb.Worksheets[0].PivotTables[0];
            pivotTable.RowFields[0].AddCalculatedItem(&quot;Test&quot;, &quot;=&apos;1&apos;&quot;);
            wb.Save(Constants.savePivottablePath + &quot;29408.xls&quot;);


        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


