---
title: TxtSaveOptions.KeepSeparatorsForBlankRow
second_title: Aspose.Cells for .NET API Reference
description: TxtSaveOptions property. Indicates whether separators should be output for blank row. Default value is false so by default the content for blank row will be empty
type: docs
url: /net/aspose.cells/txtsaveoptions/keepseparatorsforblankrow/
---
## TxtSaveOptions.KeepSeparatorsForBlankRow property

Indicates whether separators should be output for blank row. Default value is false so by default the content for blank row will be empty.

```csharp
public bool KeepSeparatorsForBlankRow { get; set; }
```

### Examples

```csharp
// Called: SaveAsCsv(wb, new TxtSaveOptions() { Encoding = Encoding.ASCII, KeepSeparatorsForBlankRow = true }));
public void TxtSaveOptions_Property_KeepSeparatorsForBlankRow()
{
    Workbook wb = new Workbook();
    Cells cells = wb.Worksheets[0].Cells;
    cells[0, 0].PutValue("a");
    cells[0, 1].PutValue("b");
    Cell cell = cells[1, 1];
    cells[3, 0].PutValue("a");
    cells[4, 1].PutValue("b");
    Assert.AreEqual("a,b\r\n,\r\n,\r\na,\r\n,b\r\n",
        SaveAsCsv(wb, new TxtSaveOptions() { Encoding = Encoding.ASCII, KeepSeparatorsForBlankRow = true }));
}
```

### See Also

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


