---
title: PivotFieldCollection.Count
second_title: Aspose.Cells for .NET API Reference
description: PivotFieldCollection property. Gets the count of the pivotFields
type: docs
url: /net/aspose.cells.pivot/pivotfieldcollection/count/
---
## PivotFieldCollection.Count property

Gets the count of the pivotFields.

```csharp
public int Count { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(80,pt.BaseFields.Count);
[Test]
        public void Property_Count()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CellsJava45720.xlsb&quot;);
            RefreshPivotTableCustomer(workbook, &quot;PivotTable1&quot;, &quot;Pivot Entry&quot;);
            //workbook.Worksheets.RefreshPivotTables();
            PivotTable pt = workbook.Worksheets[&quot;Pivot Entry&quot;].PivotTables[&quot;PivotTable1&quot;];
            Assert.AreEqual(80,pt.BaseFields.Count);
            Assert.IsTrue(pt.BaseFields[0].GroupSettings == null);
            workbook.Save(Constants.PivotTableDestPath + &quot;CellsJava45720.xlsb&quot;);
        }
```

### See Also

* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


