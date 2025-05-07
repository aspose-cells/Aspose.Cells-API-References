---
title: Style.QuotePrefix
second_title: Aspose.Cells for .NET API Reference
description: Style property. Indicates whether the cells value starts with single quote mark
type: docs
url: /net/aspose.cells/style/quoteprefix/
---
## Style.QuotePrefix property

Indicates whether the cell's value starts with single quote mark.

```csharp
public bool QuotePrefix { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(st.QuotePrefix);
[Test]
	    public void Property_QuotePrefix()
	    {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet45758.xlsb");
            Worksheet ws = workbook.Worksheets[0];

            Cell cell = ws.Cells["A1"];

            Style st = cell.GetStyle();
            Assert.IsTrue(st.QuotePrefix);
            workbook.Save(Constants.destPath + "CellsNet45758.xlsb");
            workbook = new Workbook(Constants.destPath + "CellsNet45758.xlsb");
            ws = workbook.Worksheets[0];

             cell = ws.Cells["A1"];

             st = cell.GetStyle(); 
            Assert.IsTrue(st.QuotePrefix);
            workbook.Save(Constants.destPath + "CellsNet45758.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsNet45758.xlsx");
            ws = workbook.Worksheets[0];

            cell = ws.Cells["A1"];

            st = cell.GetStyle(); 
	    }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


