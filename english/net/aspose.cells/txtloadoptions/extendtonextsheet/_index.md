---
title: TxtLoadOptions.ExtendToNextSheet
second_title: Aspose.Cells for .NET API Reference
description: TxtLoadOptions property. Whether extends data to next sheet when the rows or columns of data exceed limit. Default is false
type: docs
url: /net/aspose.cells/txtloadoptions/extendtonextsheet/
---
## TxtLoadOptions.ExtendToNextSheet property

Whether extends data to next sheet when the rows or columns of data exceed limit. Default is false.

```csharp
public bool ExtendToNextSheet { get; set; }
```

### Remarks

If this property is true, extra data will be put into next sheet behind current one (if current sheet is the last one, new sheet will be appended to current workbook). If this property is false, the data exceeding limit will be ignored.

### Examples

```csharp
// Called: ImportAsCsv(cells, 0, 0, new string(cs, 0, i + 1), new TxtLoadOptions() { ExtendToNextSheet = true });
public void TxtLoadOptions_Property_ExtendToNextSheet()
{
    char[] cs = new char[280];
    for (int i = 0; i < 20; i += 2)
    {
        cs[i] = (char)('a' + i);
        cs[i + 1] = ',';
    }
    for (int i = 20; i < 260; i++)
    {
        cs[i] = ',';
    }
    for (int i = 260; i < 280; i += 2)
    {
        cs[i] = (char)('b' + (i - 260));
        cs[i + 1] = ',';
        if (i > 264)
        {
            Workbook wb = new Workbook(FileFormatType.Excel97To2003);
            Cells cells = wb.Worksheets[0].Cells;
            ImportAsCsv(cells, 0, 0, new string(cs, 0, i + 1), new TxtLoadOptions() { ExtendToNextSheet = true });
            Assert.AreEqual(Math.Min(16, 11 + ((i - 260) >> 1)), cells.Count, "Imported cells count for " + i);
            for (int j = Math.Min((i - 260) >> 1, 6) + 249; j >= 250; j--)
            {
                Assert.AreEqual("" + (char)('b' + ((j - 250) << 1)), cells[0, j].StringValue,
                    "Col-" + j + " for " + i);
            }
            if (i > 270)
            {
                Assert.AreEqual(2, wb.Worksheets.Count, "Sheet count for " + i);
                cells = wb.Worksheets[1].Cells;
                for (int j = ((i - 260) >> 1) - 6; j >= 0; j--)
                {
                    Assert.AreEqual("" + (char)('b' + 12 + (j << 1)), cells[0, j].StringValue,
                        "ExtendedCol-" + j + " for " + i);
                }
            }
            else
            {
                Assert.AreEqual(1, wb.Worksheets.Count, "Sheet count for " + i);
            }
        }
    }
}
```

### See Also

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


