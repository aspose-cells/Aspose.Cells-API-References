---
title: Cell.IsErrorValue
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Checks if the value of this cell is an error
type: docs
url: /net/aspose.cells/cell/iserrorvalue/
---
## Cell.IsErrorValue property

Checks if the value of this cell is an error.

```csharp
public bool IsErrorValue { get; }
```

### Remarks

Also applies to formula cell to check whether the calculated result is an error.

### Examples

```csharp
// Called: Assert.IsTrue(cell.IsErrorValue, &amp;quot;Cell.IsErrorValue for SPILLERR&amp;quot;);
[Test]
        public void Property_IsErrorValue()
        { //NEED TO IMPROVE corresponding apis and then UPDATE this case
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            Cell cell = cells[0, 0];
            cell.EmbeddedImage = File.ReadAllBytes(Constants.sourcePath + &quot;1.png&quot;);
            Assert.AreEqual(&quot;#VALUE!&quot;, cell.DisplayStringValue, &quot;Cell.DisplayStringValue for SPILLERR&quot;);
            Assert.AreEqual(&quot;#VALUE!&quot;, cell.StringValue, &quot;Cell.StringValue for EmbeddedImage&quot;);
            Assert.AreEqual(&quot;#VALUE!&quot;, cell.Value, &quot;Cell.Value for EmbeddedImage&quot;); //this may be changed in later versions
            Assert.IsFalse(cell.IsErrorValue, &quot;Cell.IsErrorValue for EmbeddedImage&quot;);
            Assert.AreEqual(CellValueType.IsError, cell.Type, &quot;Cell.Type for EmbeddedImage&quot;); //this should fail
            cells[1, 0].PutValue(&quot;abc&quot;);
            cell.SetDynamicArrayFormula(&quot;=B1:B2&quot;, new FormulaParseOptions(), true);
            //Assert.AreEqual(&quot;#SPILL!&quot;, cell.DisplayStringValue, &quot;Cell.DisplayStringValue for SPILLERR&quot;);
            Assert.AreEqual(&quot;#VALUE!&quot;, cell.StringValue, &quot;Cell.StringValue for SPILLERR&quot;);
            Assert.AreEqual(&quot;#VALUE!&quot;, cell.Value, &quot;Cell.Value for SPILLERR&quot;); //this may be changed in later versions
            Assert.IsTrue(cell.IsErrorValue, &quot;Cell.IsErrorValue for SPILLERR&quot;);
            Assert.AreEqual(CellValueType.IsError, cell.Type, &quot;Cell.Type for SPILLERR&quot;);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


