---
title: TxtLoadOptions.HeaderColumnsCount
second_title: Aspose.Cells for .NET API Reference
description: TxtLoadOptions property. The count of header columns to be repeated for extended sheets
type: docs
url: /net/aspose.cells/txtloadoptions/headercolumnscount/
---
## TxtLoadOptions.HeaderColumnsCount property

The count of header columns to be repeated for extended sheets.

```csharp
public int HeaderColumnsCount { get; set; }
```

### Remarks

The header columns specified by this property will be duplicated for those extended sheets. This property only takes effect when [`ExtendToNextSheet`](../extendtonextsheet/) is true.

### Examples

```csharp
// Called: for (int c = opts.HeaderColumnsCount; c < (s < 9 ? 8 : 5); c++)
public void TxtLoadOptions_Property_HeaderColumnsCount()
{
    char[] cs = new char[450];
    for (int i = 0; i < cs.Length; i += 2)
    {
        cs[i] = i % 50 == 0 ? '\n' : ',';
        cs[i + 1] = (char)('a' + ((i >> 1) % 26));
    }
    string content = new string(cs, 1, cs.Length - 1);
    TxtLoadOptions opts = new TxtLoadOptions()
    {
        Encoding = Encoding.Unicode,
        ExtendToNextSheet = true,
        HeaderRowsCount = 2,
        HeaderColumnsCount = 3,
        MaxRowCount = 6,
        MaxColumnCount = 8
    };
    MemoryStream ms = new MemoryStream(Encoding.Unicode.GetBytes(content), false);
    Workbook wb = new Workbook(ms, opts);
    int tailRow = cs.Length / 50 - opts.MaxRowCount;
    int tailCol = opts.MaxRowCount - opts.HeaderRowsCount;
    int sheetCount = (tailRow + tailCol - 1) / tailCol + 1;
    tailRow = (tailRow % tailCol) + opts.HeaderRowsCount;
    tailCol = opts.MaxColumnCount - opts.HeaderColumnsCount;
    sheetCount *= (25 - opts.MaxColumnCount + tailCol - 1) / tailCol + 1;
    tailCol = ((25 - opts.MaxColumnCount) % tailCol) + opts.HeaderColumnsCount;
    Assert.AreEqual(sheetCount, wb.Worksheets.Count, "Data should be expanded to 10 sheets");
    Cells cells;
    string sn;
    for (int s = 0; s < (sheetCount >> 1); s++)
    {
        cells = wb.Worksheets[s].Cells;
        sn = "Sheet" + (s + 1) + "!";
        for (int r = 0; r < opts.MaxRowCount; r++)
        {
            for (int c = 0; c < opts.HeaderColumnsCount; c++)
            {
                Assert.AreEqual("" + (char)('a' + (r * 25 + c) % 26), cells[r, c].StringValue,
                    sn + CellsHelper.CellIndexToName(r, c));
            }
            for (int c = opts.HeaderColumnsCount; c < (s < 4 ? 8 : 5); c++)
            {
                Assert.AreEqual("" + (char)('a' + (26 - r + s * 5 + c) % 26), cells[r, c].StringValue,
                    sn + CellsHelper.CellIndexToName(r, c));
            }
        }
    }
    for (int s = (sheetCount >> 1); s < sheetCount; s++)
    {
        cells = wb.Worksheets[s].Cells;
        sn = "Sheet" + (s + 1) + "!";
        for (int r = 0; r < opts.HeaderRowsCount; r++)
        {
            for (int c = 0; c < opts.HeaderColumnsCount; c++)
            {
                Assert.AreEqual("" + (char)('a' + (r * 25 + c) % 26), cells[r, c].StringValue,
                    sn + CellsHelper.CellIndexToName(r, c));
            }
            for (int c = opts.HeaderColumnsCount; c < (s < 9 ? 8 : 5); c++)
            {
                Assert.AreEqual("" + (char)('a' + (1 - r + s * 5 + c) % 26), cells[r, c].StringValue,
                    sn + CellsHelper.CellIndexToName(r, c));
            }
        }
        for (int r = opts.HeaderRowsCount; r < tailRow; r++)
        {
            for (int c = 0; c < opts.HeaderColumnsCount; c++)
            {
                Assert.AreEqual("" + (char)('a' + (r * 25 + c - 4) % 26), cells[r, c].StringValue,
                    sn + CellsHelper.CellIndexToName(r, c));
            }
            for (int c = opts.HeaderColumnsCount; c < (s < 9 ? 8 : 5); c++)
            {
                Assert.AreEqual("" + (char)('a' + (23 - r + s * 5 + c) % 26), cells[r, c].StringValue,
                    sn + CellsHelper.CellIndexToName(r, c));
            }
        }
    }

    wb = new Workbook(FileFormatType.Excel97To2003);
    ms.Seek(0, SeekOrigin.Begin);
    wb.Worksheets[0].Cells.ImportCSV(ms, opts, 65532, 252);

    sheetCount = 16;
    cells = wb.Worksheets[0].Cells;
    sn = "Sheet1!";
    for (int r = 65532; r < 65536; r++)
    {
        for (int c = 252; c < 256; c++)
        {
            Assert.AreEqual("" + (char)('a' + ((r - 65532) * 25 + c - 252) % 26),
                cells[r, c].StringValue, sn + CellsHelper.CellIndexToName(r, c));
        }
    }
    for (int s = 1; s < 6; s++)
    {
        cells = wb.Worksheets[s].Cells;
        sn = "Sheet" + (s + 1) + "!";
        for (int r = 0; r < 4; r++)
        {
            for (int c = 0; c < opts.HeaderColumnsCount; c++)
            {
                Assert.AreEqual("" + (char)('a' + (r * 25 + c) % 26), cells[r, c].StringValue,
                    sn + CellsHelper.CellIndexToName(r, c));
            }
            for (int c = opts.HeaderColumnsCount; c < (s < 5 ? 8 : 4); c++)
            {
                Assert.AreEqual("" + (char)('a' + (22 - r + s * 5 + c) % 26), cells[r, c].StringValue,
                    sn + CellsHelper.CellIndexToName(r, c));
            }
        }
    }
    cells = wb.Worksheets[5].Cells;
    sn = "Sheet6!";
    for (int r = 0; r < 4; r++)
    {
        for (int c = 0; c < opts.HeaderColumnsCount; c++)
        {
            Assert.AreEqual("" + (char)('a' + (r * 25 + c) % 26), cells[r, c].StringValue,
                sn + CellsHelper.CellIndexToName(r, c));
        }
        Assert.AreEqual("" + (char)('y' - r), cells[r, opts.HeaderColumnsCount].StringValue,
            sn + CellsHelper.CellIndexToName(r, opts.HeaderColumnsCount));
    }
    for (int s = 6; s < 11; s++)
    {
        cells = wb.Worksheets[s].Cells;
        sn = "Sheet" + (s + 1) + "!";
        for (int r = 0; r < opts.HeaderRowsCount; r++)
        {
            for (int c = 0; c < opts.HeaderColumnsCount; c++)
            {
                Assert.AreEqual("" + (char)('a' + (r * 25 + c) % 26), cells[r, c].StringValue,
                    sn + CellsHelper.CellIndexToName(r, c));
            }
            for (int c = opts.HeaderColumnsCount; c < (s < 10 ? 8 : 5); c++)
            {
                Assert.AreEqual("" + (char)('a' + (s * 5 + c - 30 - r) % 26), cells[r, c].StringValue,
                    sn + CellsHelper.CellIndexToName(r, c));
            }
        }
        for (int r = opts.HeaderRowsCount; r < 6; r++)
        {
            for (int c = 0; c < opts.HeaderColumnsCount; c++)
            {
                Assert.AreEqual("" + (char)('a' + (r * 25 + c - 28) % 26), cells[r, c].StringValue,
                    sn + CellsHelper.CellIndexToName(r, c));
            }
            for (int c = opts.HeaderColumnsCount; c < (s < 10 ? 8 : 5); c++)
            {
                Assert.AreEqual("" + (char)('a' + ((s - 6) * 5 + r * 25 + c - 2) % 26), cells[r, c].StringValue,
                    sn + CellsHelper.CellIndexToName(r, c));
            }
        }
    }
    for (int s = 11; s < 16; s++)
    {
        cells = wb.Worksheets[s].Cells;
        sn = "Sheet" + (s + 1) + "!";
        for (int r = 0; r < opts.HeaderRowsCount; r++)
        {
            for (int c = 0; c < opts.HeaderColumnsCount; c++)
            {
                Assert.AreEqual("" + (char)('a' + (r * 25 + c) % 26), cells[r, c].StringValue,
                    sn + CellsHelper.CellIndexToName(r, c));
            }
            for (int c = opts.HeaderColumnsCount; c < (s < 15 ? 8 : 5); c++)
            {
                Assert.AreEqual("" + (char)('a' + (s * 5 + c - 29 - r) % 26), cells[r, c].StringValue,
                    sn + CellsHelper.CellIndexToName(r, c));
            }
        }
        for (int c = 0; c < opts.HeaderColumnsCount; c++)
        {
            Assert.AreEqual("" + (char)('a' + (18 + c) % 26), cells[2, c].StringValue,
                sn + CellsHelper.CellIndexToName(2, c));
        }
        for (int c = opts.HeaderColumnsCount; c < (s < 15 ? 8 : 5); c++)
        {
            Assert.AreEqual("" + (char)('a' + ((s - 6) * 5 + 19 + c) % 26), cells[2, c].StringValue,
                sn + CellsHelper.CellIndexToName(2, c));
        }
    }
}
```

### See Also

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


