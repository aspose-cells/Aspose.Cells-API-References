---
title: Font.IsBold
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets or sets a value indicating whether the font is bold
type: docs
url: /net/aspose.cells/font/isbold/
---
## Font.IsBold property

Gets or sets a value indicating whether the font is bold.

```csharp
public bool IsBold { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(true, cells[&amp;quot;A12&amp;quot;].GetStyle().Font.IsBold);
[Test]
        public void Property_IsBold()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;Numbers13/NFD-MEAT-TEMPLATE-input.numbers&quot;);
            wb = Util.ReSave(wb, SaveFormat.Xlsx);
            Cells cells = wb.Worksheets[0].Cells;
            Assert.AreEqual(&quot;FROZEN TURKEYS&quot;, cells[&quot;A12&quot;].StringValue);
            Assert.AreEqual(true, cells[&quot;A12&quot;].GetStyle().Font.IsBold);
            Assert.AreEqual(true, cells[&quot;A12&quot;].GetStyle().Font.IsItalic);
            DateTime dt = new DateTime(2023, 11, 13);
            Assert.AreEqual(dt, cells[&quot;M16&quot;].DateTimeValue);
            dt = new DateTime(2023, 10, 19);
            Assert.AreEqual(dt, cells[&quot;B2&quot;].DateTimeValue);
            //Assert.AreEqual(&quot;&quot;, cells[&quot;M16&quot;].DateTimeValue);
            Assert.AreEqual(&quot;1.00&quot;, cells[&quot;G42&quot;].StringValue);
            Assert.AreEqual(&quot;POULTRY&quot;, cells[&quot;A29&quot;].StringValue);
            Assert.AreEqual(&quot;PORK&quot;, cells[&quot;A32&quot;].StringValue);
            Assert.AreEqual(&quot;MISC.&quot;, cells[&quot;A52&quot;].StringValue);
            Assert.AreEqual(&quot;FROZEN BUTTERBALL SMOKED TURKEY        (9.5-13LB. AVG) &quot;, cells[&quot;B20&quot;].StringValue);
            Assert.AreEqual(&quot;Account #&quot;, cells[&quot;I61&quot;].StringValue);
        }
```

### See Also

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


