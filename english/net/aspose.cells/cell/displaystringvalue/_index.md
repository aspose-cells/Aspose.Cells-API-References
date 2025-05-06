---
title: Cell.DisplayStringValue
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets the formatted string value of this cell by cells display style
type: docs
url: /net/aspose.cells/cell/displaystringvalue/
---
## Cell.DisplayStringValue property

Gets the formatted string value of this cell by cell's display style.

```csharp
public string DisplayStringValue { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;0.1&amp;quot;, cell.DisplayStringValue, &amp;quot;Value 0.14 with ColumnWidth 3&amp;quot;);
[Test]
        public void Property_DisplayStringValue()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            Cell cell = cells[0, 0];
            cells.SetColumnWidth(0, 1);
            cell.PutValue(0.4);
            Assert.AreEqual(&quot;0&quot;, cell.DisplayStringValue, &quot;Value 0.4 with ColumnWidth 1&quot;);
            cell.PutValue(0.5);
            Assert.AreEqual(&quot;1&quot;, cell.DisplayStringValue, &quot;Value 0.5 with ColumnWidth 1&quot;);
            cell.PutValue(1.4);
            Assert.AreEqual(&quot;1&quot;, cell.DisplayStringValue, &quot;Value 1.4 with ColumnWidth 1&quot;);
            cell.PutValue(1.5);
            Assert.AreEqual(&quot;2&quot;, cell.DisplayStringValue, &quot;Value 1.5 with ColumnWidth 1&quot;);
            cell.PutValue(0.04);
            Assert.AreEqual(&quot;0&quot;, cell.DisplayStringValue, &quot;Value 0.04 with ColumnWidth 1&quot;);
            cell.PutValue(0.05);
            Assert.AreEqual(&quot;0&quot;, cell.DisplayStringValue, &quot;Value 0.05 with ColumnWidth 1&quot;);
            cells.SetColumnWidth(0, 2);
            cell.PutValue(0.4);
            Assert.AreEqual(&quot;0&quot;, cell.DisplayStringValue, &quot;Value 0.4 with ColumnWidth 2&quot;);
            cell.PutValue(0.5);
            Assert.AreEqual(&quot;1&quot;, cell.DisplayStringValue, &quot;Value 0.5 with ColumnWidth 2&quot;);
            cell.PutValue(1.4);
            Assert.AreEqual(&quot;1&quot;, cell.DisplayStringValue, &quot;Value 1.4 with ColumnWidth 2&quot;);
            cell.PutValue(1.5);
            Assert.AreEqual(&quot;2&quot;, cell.DisplayStringValue, &quot;Value 1.5 with ColumnWidth 2&quot;);
            cell.PutValue(0.04);
            Assert.AreEqual(&quot;0&quot;, cell.DisplayStringValue, &quot;Value 0.04 with ColumnWidth 2&quot;);
            cell.PutValue(0.05);
            Assert.AreEqual(&quot;0&quot;, cell.DisplayStringValue, &quot;Value 0.05 with ColumnWidth 2&quot;);
            cells.SetColumnWidth(0, 3);
            cell.PutValue(0.4);
            Assert.AreEqual(&quot;0.4&quot;, cell.DisplayStringValue, &quot;Value 0.4 with ColumnWidth 3&quot;);
            cell.PutValue(0.5);
            Assert.AreEqual(&quot;0.5&quot;, cell.DisplayStringValue, &quot;Value 0.5 with ColumnWidth 3&quot;);
            cell.PutValue(0.14);
            Assert.AreEqual(&quot;0.1&quot;, cell.DisplayStringValue, &quot;Value 0.14 with ColumnWidth 3&quot;);
            cell.PutValue(0.15);
            Assert.AreEqual(&quot;0.2&quot;, cell.DisplayStringValue, &quot;Value 0.15 with ColumnWidth 3&quot;);
            cell.PutValue(0.04);
            Assert.AreEqual(&quot;0&quot;, cell.DisplayStringValue, &quot;Value 0.04 with ColumnWidth 3&quot;);
            cell.PutValue(0.05);
            Assert.AreEqual(&quot;0.1&quot;, cell.DisplayStringValue, &quot;Value 0.05 with ColumnWidth 3&quot;);
            cell.PutValue(0.004);
            Assert.AreEqual(&quot;0&quot;, cell.DisplayStringValue, &quot;Value 0.004 with ColumnWidth 3&quot;);
            cell.PutValue(0.005);
            Assert.AreEqual(&quot;0&quot;, cell.DisplayStringValue, &quot;Value 0.005 with ColumnWidth 3&quot;);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


