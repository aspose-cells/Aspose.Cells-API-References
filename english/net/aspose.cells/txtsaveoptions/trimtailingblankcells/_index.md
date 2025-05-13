---
title: TxtSaveOptions.TrimTailingBlankCells
second_title: Aspose.Cells for .NET API Reference
description: TxtSaveOptions property. Indicates whether tailing blank cells in one row should be trimmed. Default is false
type: docs
url: /net/aspose.cells/txtsaveoptions/trimtailingblankcells/
---
## TxtSaveOptions.TrimTailingBlankCells property

Indicates whether tailing blank cells in one row should be trimmed. Default is false.

```csharp
public bool TrimTailingBlankCells { get; set; }
```

### Remarks

When saving with LightCells mode and the [`ExportArea`](../exportarea/) has not been specified, this option takes no effect and one row will be extended to just the last cell provided by the implementation [`LightCellsDataProvider`](../lightcellsdataprovider/)

### Examples

```csharp
// Called: TrimTailingBlankCells = true,
public void TxtSaveOptions_Property_TrimTailingBlankCells()
{
    Workbook wb = new Workbook();
    Cells cells = wb.Worksheets[0].Cells;
    cells[1, 1].PutValue(1);
    cells[2, 1].PutValue(2);
    cells[3, 1].PutValue(3);
    cells[3, 3].PutValue(4);
    cells[4, 1].PutValue(5);
    Assert.AreEqual("1,,\r\n2,,\r\n3,,4\r\n5,,\r\n",
        SaveAsCsv(wb, new TxtSaveOptions() { Encoding = Encoding.ASCII }), "All default");
    Assert.AreEqual(",,,\r\n,1,,\r\n,2,,\r\n,3,,4\r\n,5,,\r\n",
        SaveAsCsv(wb, new TxtSaveOptions()
        {
            Encoding = Encoding.ASCII,
            TrimLeadingBlankRowAndColumn = false,
            KeepSeparatorsForBlankRow = true
        }), "NoTrimHead, KeepSep");
    ;
    Assert.AreEqual("\r\n,1,,\r\n,2,,\r\n,3,,4\r\n,5,,\r\n",
        SaveAsCsv(wb, new TxtSaveOptions()
        {
            Encoding = Encoding.ASCII,
            TrimLeadingBlankRowAndColumn = false,
        }), "NoTrimHead, NoKeepSep");
    ;
    Style style = wb.CreateStyle();
    style.Font.Size = 26;
    StyleFlag sf = new StyleFlag();
    sf.All = true;
    cells.Columns[0].ApplyStyle(style, sf);
    Assert.AreEqual(",1,,\r\n,2,,\r\n,3,,4\r\n,5,,\r\n",
        SaveAsCsv(wb, new TxtSaveOptions() { Encoding = Encoding.ASCII }), "AddColumnStyle");
    cells.Rows[0].ApplyStyle(style, sf);
    Assert.AreEqual("\r\n,1,,\r\n,2,,\r\n,3,,4\r\n,5,,\r\n",
        SaveAsCsv(wb, new TxtSaveOptions() { Encoding = Encoding.ASCII }), "AddRowStyle");
    Assert.AreEqual("\r\n,1\r\n,2\r\n,3,,4\r\n,5\r\n",
        SaveAsCsv(wb, new TxtSaveOptions()
        {
            Encoding = Encoding.ASCII,
            TrimTailingBlankCells = true
        }), "TrimTail");
    Assert.AreEqual(",,,\r\n,1\r\n,2\r\n,3,,4\r\n,5\r\n",
        SaveAsCsv(wb, new TxtSaveOptions()
        {
            Encoding = Encoding.ASCII,
            TrimTailingBlankCells = true,
            KeepSeparatorsForBlankRow = true
        }), "TrimTail, KeepSep");
}
```

### See Also

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


