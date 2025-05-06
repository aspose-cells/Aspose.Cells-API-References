---
title: TxtSaveOptions.Encoding
second_title: Aspose.Cells for .NET API Reference
description: TxtSaveOptions property. Gets and sets the default encoding
type: docs
url: /net/aspose.cells/txtsaveoptions/encoding/
---
## TxtSaveOptions.Encoding property

Gets and sets the default encoding.

```csharp
public Encoding Encoding { get; set; }
```

### Examples

```csharp
// Called: Encoding = Encoding.ASCII,
[Test]
        public void Property_Encoding()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            cells[1, 1].PutValue(1);
            cells[2, 1].PutValue(2);
            cells[3, 1].PutValue(3);
            cells[3, 3].PutValue(4);
            cells[4, 1].PutValue(5);
            Assert.AreEqual(&quot;1,,\r\n2,,\r\n3,,4\r\n5,,\r\n&quot;,
                SaveAsCsv(wb, new TxtSaveOptions() { Encoding = Encoding.ASCII }), &quot;All default&quot;);
            Assert.AreEqual(&quot;,,,\r\n,1,,\r\n,2,,\r\n,3,,4\r\n,5,,\r\n&quot;,
                SaveAsCsv(wb, new TxtSaveOptions()
                {
                    Encoding = Encoding.ASCII,
                    TrimLeadingBlankRowAndColumn = false,
                    KeepSeparatorsForBlankRow = true
                }), &quot;NoTrimHead, KeepSep&quot;);
            ;
            Assert.AreEqual(&quot;\r\n,1,,\r\n,2,,\r\n,3,,4\r\n,5,,\r\n&quot;,
                SaveAsCsv(wb, new TxtSaveOptions()
                {
                    Encoding = Encoding.ASCII,
                    TrimLeadingBlankRowAndColumn = false,
                }), &quot;NoTrimHead, NoKeepSep&quot;);
            ;
            Style style = wb.CreateStyle();
            style.Font.Size = 26;
            StyleFlag sf = new StyleFlag();
            sf.All = true;
            cells.Columns[0].ApplyStyle(style, sf);
            Assert.AreEqual(&quot;,1,,\r\n,2,,\r\n,3,,4\r\n,5,,\r\n&quot;,
                SaveAsCsv(wb, new TxtSaveOptions() { Encoding = Encoding.ASCII }), &quot;AddColumnStyle&quot;);
            cells.Rows[0].ApplyStyle(style, sf);
            Assert.AreEqual(&quot;\r\n,1,,\r\n,2,,\r\n,3,,4\r\n,5,,\r\n&quot;,
                SaveAsCsv(wb, new TxtSaveOptions() { Encoding = Encoding.ASCII }), &quot;AddRowStyle&quot;);
            Assert.AreEqual(&quot;\r\n,1\r\n,2\r\n,3,,4\r\n,5\r\n&quot;,
                SaveAsCsv(wb, new TxtSaveOptions()
                {
                    Encoding = Encoding.ASCII,
                    TrimTailingBlankCells = true
                }), &quot;TrimTail&quot;);
            Assert.AreEqual(&quot;,,,\r\n,1\r\n,2\r\n,3,,4\r\n,5\r\n&quot;,
                SaveAsCsv(wb, new TxtSaveOptions()
                {
                    Encoding = Encoding.ASCII,
                    TrimTailingBlankCells = true,
                    KeepSeparatorsForBlankRow = true
                }), &quot;TrimTail, KeepSep&quot;);
        }
```

### See Also

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


