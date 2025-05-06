---
title: Cell.IsMerged
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Checks if a cell is part of a merged range or not
type: docs
url: /net/aspose.cells/cell/ismerged/
---
## Cell.IsMerged property

Checks if a cell is part of a merged range or not.

```csharp
public bool IsMerged { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(true, cells[&amp;quot;C4&amp;quot;].IsMerged);
[Test]
        public void Property_IsMerged()
        {
            Workbook wb = new Workbook(Constants.sourcePath + @&quot;Numbers13\ExpTest\CellsMerge.xlsx&quot;);
#if APPLECHECK
            wb.Save(Constants.sourcePath + @&quot;Numbers13\ExpTest\CellsMerge_Ret.numbers&quot;);
#endif
            Workbook numbers = Util.ReSave(wb, SaveFormat.Numbers);
            Cells cells = numbers.Worksheets[0].Cells;
            Assert.AreEqual(CellValueType.IsString, cells[&quot;C4&quot;].Type);
            Assert.AreEqual(&quot;AA&quot;, cells[&quot;C4&quot;].StringValue);
            Assert.AreEqual(TextAlignmentType.Left, cells[&quot;C4&quot;].GetStyle().HorizontalAlignment);
            Assert.AreEqual(TextAlignmentType.Bottom, cells[&quot;C4&quot;].GetStyle().VerticalAlignment);
            Assert.AreEqual(true, cells[&quot;C4&quot;].IsMerged);
            Assert.AreEqual(true, cells[&quot;C5&quot;].IsMerged);
            Assert.AreEqual(true, cells[&quot;D4&quot;].IsMerged);
            Assert.AreEqual(true, cells[&quot;D5&quot;].IsMerged);


            Assert.AreEqual(CellValueType.IsString, cells[&quot;E8&quot;].Type);
            Assert.AreEqual(&quot;BB&quot;, cells[&quot;E8&quot;].StringValue);
            Assert.AreEqual(true, cells[&quot;E8&quot;].IsMerged);
            Assert.AreEqual(true, cells[&quot;E9&quot;].IsMerged);
            Assert.AreEqual(true, cells[&quot;F8&quot;].IsMerged);
            Assert.AreEqual(true, cells[&quot;F9&quot;].IsMerged);

            cells = numbers.Worksheets[1].Cells;
            Assert.AreEqual(CellValueType.IsString, cells[&quot;C4&quot;].Type);
            Assert.AreEqual(&quot;CC&quot;, cells[&quot;C4&quot;].StringValue);
            Assert.AreEqual(true, cells[&quot;C4&quot;].IsMerged);
            Assert.AreEqual(true, cells[&quot;C5&quot;].IsMerged);
            Assert.AreEqual(true, cells[&quot;C6&quot;].IsMerged);
            Assert.AreEqual(true, cells[&quot;D4&quot;].IsMerged);
            Assert.AreEqual(true, cells[&quot;D5&quot;].IsMerged);
            Assert.AreEqual(true, cells[&quot;D6&quot;].IsMerged);
            Assert.AreEqual(true, cells[&quot;E4&quot;].IsMerged);
            Assert.AreEqual(true, cells[&quot;E5&quot;].IsMerged);
            Assert.AreEqual(true, cells[&quot;E6&quot;].IsMerged);
            Assert.AreEqual(TextAlignmentType.Right, cells[&quot;C4&quot;].GetStyle().HorizontalAlignment);
            Assert.AreEqual(TextAlignmentType.Bottom, cells[&quot;C4&quot;].GetStyle().VerticalAlignment);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


