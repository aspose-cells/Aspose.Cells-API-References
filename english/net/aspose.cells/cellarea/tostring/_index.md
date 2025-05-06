---
title: CellArea.ToString
second_title: Aspose.Cells for .NET API Reference
description: CellArea method. Returns a string represents the current cell area object
type: docs
url: /net/aspose.cells/cellarea/tostring/
---
## CellArea.ToString method

Returns a string represents the current cell area object.

```csharp
public override string ToString()
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;Aspose.Cells.CellArea(F9:G11)[8,5,10,6]&amp;quot;, ca.ToString());
[Test]
        public void Method_ToString()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET48649.xlsx&quot;);

            workbook.Save(Constants.destPath + &quot;CELLSNET48649.ods&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET48649.ods&quot;);

            CellArea[] areas = workbook.Worksheets[0].Cells.GetMergedAreas();
           Assert.AreEqual(3,areas.Length);
            CellArea ca = (CellArea)areas[0];
            Assert.AreEqual(&quot;Aspose.Cells.CellArea(C4:D6)[3,2,5,3]&quot;, ca.ToString());
            ca = (CellArea)areas[1];
            Assert.AreEqual(&quot;Aspose.Cells.CellArea(F9:G11)[8,5,10,6]&quot;, ca.ToString());
 
             ca = (CellArea)areas[2];
            Assert.AreEqual(&quot;Aspose.Cells.CellArea(C10:D15)[9,2,14,3]&quot;, ca.ToString());
            workbook.Save(Constants.destPath + &quot;CELLSNET48649.xlsx&quot;);
        }
```

### See Also

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


