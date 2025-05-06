---
title: Cell.R1C1Formula
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets or sets a R1C1 formula of the Cell
type: docs
url: /net/aspose.cells/cell/r1c1formula/
---
## Cell.R1C1Formula property

Gets or sets a R1C1 formula of the [`Cell`](../).

```csharp
public string R1C1Formula { get; set; }
```

### Examples

```csharp
// Called: string b1 = wk.Worksheets[0].Cells[&amp;quot;B1&amp;quot;].R1C1Formula;
[Test]
	    public void Property_R1C1Formula()
	    {
            Workbook wk = new Workbook(Constants.sourcePath + &quot;Formula/CellsJava42111.xlsx&quot;);
            string a1 = wk.Worksheets[0].Cells[&quot;A1&quot;].R1C1Formula;
            string b1 = wk.Worksheets[0].Cells[&quot;B1&quot;].R1C1Formula;
            string a2 = wk.Worksheets[0].Cells[&quot;A2&quot;].R1C1Formula;
            string b2 = wk.Worksheets[0].Cells[&quot;B2&quot;].R1C1Formula;
            Assert.AreEqual(a1, &quot;=R[1048575]C&quot;);
            Assert.AreEqual(b1,&quot;=R[1048574]C&quot;);
            Assert.AreEqual(a2, &quot;=R1048576C&quot;);
            Assert.AreEqual(b2, &quot;=R1048575C&quot;);
            //      wk.Worksheets[0].Cells.DeleteRows(17, 9);
            string a11 = CellsHelper.ConvertR1C1FormulaToA1(a1, 0, 0);
            string a22 = CellsHelper.ConvertR1C1FormulaToA1(a2, 0, 0);
            string b11 = CellsHelper.ConvertR1C1FormulaToA1(b1, 0, 1);
            string b22 = CellsHelper.ConvertR1C1FormulaToA1(b2, 0, 1);
            Assert.AreEqual(a11, &quot;=A1048576&quot;);
            Assert.AreEqual(b11, &quot;=B1048575&quot;);
            Assert.AreEqual(a22, &quot;=A$1048576&quot;);
            Assert.AreEqual(b22, &quot;=B$1048575&quot;);
	    }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


