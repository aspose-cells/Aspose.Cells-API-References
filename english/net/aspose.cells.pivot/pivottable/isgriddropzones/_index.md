---
title: PivotTable.IsGridDropZones
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether the PivotTable report displays classic pivottable layout. enables dragging fields in the grid
type: docs
url: /net/aspose.cells.pivot/pivottable/isgriddropzones/
---
## PivotTable.IsGridDropZones property

Indicates whether the PivotTable report displays classic pivottable layout. (enables dragging fields in the grid)

```csharp
public bool IsGridDropZones { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(first, wb.Worksheets[&amp;quot;Report&amp;quot;].PivotTables[0].IsGridDropZones);
[Test]
        public void Property_IsGridDropZones()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;JAVA41530_&quot;;

            Workbook wb = new Workbook(filePath + &quot;pivot.xlsb&quot;);
            bool first = wb.Worksheets[&quot;Report&quot;].PivotTables[0].IsGridDropZones;
            wb.Save(Constants.PivotTableDestPath + @&quot;JAVA41530.xlsb&quot;);

            wb = new Workbook(Constants.PivotTableDestPath + @&quot;JAVA41530.xlsb&quot;);
            Assert.AreEqual(first, wb.Worksheets[&quot;Report&quot;].PivotTables[0].IsGridDropZones);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


