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
// Called: Assert.AreEqual(wb.Worksheets[0].Cells["C4"].Formula, wb.Worksheets[0].Cells["C4"].R1C1Formula);
	    public void Cell_Property_R1C1Formula()
	    {
            Workbook wb = new Workbook(Constants.sourcePath + "example.xlsm");
            Assert.AreEqual(wb.Worksheets[0].Cells["C4"].Formula,wb.Worksheets[0].Cells["C4"].R1C1Formula);
            wb = Util.ReSave(wb, SaveFormat.Xlsm);
            Assert.AreEqual(wb.Worksheets[0].Cells["C4"].Formula, wb.Worksheets[0].Cells["C4"].R1C1Formula);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


