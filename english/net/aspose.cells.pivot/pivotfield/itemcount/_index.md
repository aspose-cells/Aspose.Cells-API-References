---
title: PivotField.ItemCount
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Gets the count of the base items in this pivot field
type: docs
url: /net/aspose.cells.pivot/pivotfield/itemcount/
---
## PivotField.ItemCount property

Gets the count of the base items in this pivot field.

```csharp
public int ItemCount { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(pt.RowFields[0].ItemCount, 4);
[Test]
        public void Property_ItemCount()
        {
            var wb = new Workbook(Constants.openPivottablePath + &quot;testBaseItemSubtotal.xlsx&quot;);
            PivotTable pt = wb.Worksheets[1].PivotTables[0];
            //Console.WriteLine(pt.PageFieldWrapCount);
            //Console.WriteLine(pt.DisplayNullString);
            //Console.WriteLine(pt.PreserveFormatting);
            //Console.WriteLine(pt.ItemPrintTitles);
            
            Assert.AreEqual(pt.RowFields[0].ItemCount, 4);
            //wb.Save(&quot;D:\\40095.xlsx&quot;);
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


