---
title: Style.HorizontalAlignment
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets or sets the horizontal alignment type of the text in a cell
type: docs
url: /net/aspose.cells/style/horizontalalignment/
---
## Style.HorizontalAlignment property

Gets or sets the horizontal alignment type of the text in a cell.

```csharp
public TextAlignmentType HorizontalAlignment { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(TextAlignmentType.Left, style.HorizontalAlignment);
[Test]
        public void Property_HorizontalAlignment()
        {
            Workbook wb = new Workbook(Constants.sourcePath + @&quot;Numbers13\ExpTest\Alignment.xlsx&quot;);
#if APPLECHECK
            wb.Save(Constants.sourcePath + @&quot;Numbers13\ExpTest\Alignment_Ret.numbers&quot;);
#endif
            //wb = new Workbook(Constants.sourcePath + @&quot;Numbers13\ExpTest\Alignment_Ret.numbers&quot;);
            //wb.Save(Constants.sourcePath + @&quot;Numbers13\ExpTest\Alignment_Ret.xlsx&quot;);
            Workbook numbers = Util.ReSave(wb, SaveFormat.Numbers);
            Cells cells = numbers.Worksheets[0].Cells;
            //sheet1 E7
            Cell E7Cell = cells[&quot;E7&quot;];
            Assert.AreEqual(CellValueType.IsString, E7Cell.Type);
            Assert.AreEqual(&quot;a&quot;, E7Cell.StringValue);
            Style style = E7Cell.GetStyle();
            Assert.AreEqual(11, style.Font.Size);
            Assert.AreEqual(TextAlignmentType.Center, style.VerticalAlignment);
            Assert.AreEqual(TextAlignmentType.Left, style.HorizontalAlignment);

            //F7
            Cell F7Cell = cells[&quot;F7&quot;];
            Assert.AreEqual(CellValueType.IsString, F7Cell.Type);
            Assert.AreEqual(&quot;b&quot;, F7Cell.StringValue);
            style = F7Cell.GetStyle();
            Assert.AreEqual(11, style.Font.Size);
            Assert.AreEqual(TextAlignmentType.Top, style.VerticalAlignment);
            Assert.AreEqual(TextAlignmentType.Left, style.HorizontalAlignment);

            //G7
            Cell G7Cell = cells[&quot;G7&quot;];
            Assert.AreEqual(CellValueType.IsString, G7Cell.Type);
            Assert.AreEqual(&quot;c&quot;, G7Cell.StringValue);
            style = G7Cell.GetStyle();
            Assert.AreEqual(11, style.Font.Size);
            Assert.AreEqual(TextAlignmentType.Top, style.VerticalAlignment);
            Assert.AreEqual(TextAlignmentType.Center, style.HorizontalAlignment);

            //H7
            Cell H7Cell = cells[&quot;H7&quot;];
            Assert.AreEqual(CellValueType.IsString, H7Cell.Type);
            Assert.AreEqual(&quot;d&quot;, H7Cell.StringValue);
            style = H7Cell.GetStyle();
            Assert.AreEqual(TextAlignmentType.Top, style.VerticalAlignment);
            Assert.AreEqual(TextAlignmentType.Right, style.HorizontalAlignment);

            //I7
            Cell I7Cell = cells[&quot;I7&quot;];
            Assert.AreEqual(CellValueType.IsString, I7Cell.Type);
            Assert.AreEqual(&quot;e&quot;, I7Cell.StringValue);
            style = I7Cell.GetStyle();
            Assert.AreEqual(TextAlignmentType.Center, style.VerticalAlignment);
            Assert.AreEqual(TextAlignmentType.Right, style.HorizontalAlignment);

            //J7
            Cell J7Cell = cells[&quot;J7&quot;];
            Assert.AreEqual(CellValueType.IsString, J7Cell.Type);
            Assert.AreEqual(&quot;f&quot;, J7Cell.StringValue);
            style = J7Cell.GetStyle();
            Assert.AreEqual(TextAlignmentType.Bottom, style.VerticalAlignment);
            Assert.AreEqual(TextAlignmentType.Right, style.HorizontalAlignment);

            //K7
            Cell K7Cell = cells[&quot;K7&quot;];
            Assert.AreEqual(CellValueType.IsString, K7Cell.Type);
            Assert.AreEqual(&quot;g&quot;, K7Cell.StringValue);
            style = K7Cell.GetStyle();
            Assert.AreEqual(TextAlignmentType.Bottom, style.VerticalAlignment);
            Assert.AreEqual(TextAlignmentType.Center, style.HorizontalAlignment);

            //L7
            Cell L7Cell = cells[&quot;L7&quot;];
            Assert.AreEqual(CellValueType.IsString, L7Cell.Type);
            Assert.AreEqual(&quot;h&quot;, L7Cell.StringValue);
            style = L7Cell.GetStyle();
            Assert.AreEqual(TextAlignmentType.Bottom, style.VerticalAlignment);
            Assert.AreEqual(TextAlignmentType.Left, style.HorizontalAlignment);

            //M7
            Cell M7Cell = cells[&quot;M7&quot;];
            Assert.AreEqual(CellValueType.IsString, M7Cell.Type);
            Assert.AreEqual(&quot;a&quot;, M7Cell.StringValue);
            style = M7Cell.GetStyle();
            Assert.AreEqual(TextAlignmentType.Center, style.VerticalAlignment);
            Assert.AreEqual(TextAlignmentType.Left, style.HorizontalAlignment);

            //sheet2 E10
            cells = numbers.Worksheets[1].Cells;
            Cell E10Cell = cells[&quot;E10&quot;];
            Assert.AreEqual(CellValueType.IsString, E10Cell.Type);
            Assert.AreEqual(&quot;b&quot;, E10Cell.StringValue);
            style = E10Cell.GetStyle();
            Assert.AreEqual(11, style.Font.Size);
            Assert.AreEqual(TextAlignmentType.Bottom, style.VerticalAlignment);
            Assert.AreEqual(TextAlignmentType.Left, style.HorizontalAlignment);
        }
```

### See Also

* enum [TextAlignmentType](../../textalignmenttype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


