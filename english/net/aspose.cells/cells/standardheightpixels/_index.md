---
title: Cells.StandardHeightPixels
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets or sets the default row height in this worksheet in unit of pixels
type: docs
url: /net/aspose.cells/cells/standardheightpixels/
---
## Cells.StandardHeightPixels property

Gets or sets the default row height in this worksheet, in unit of pixels.

```csharp
public int StandardHeightPixels { get; set; }
```

### Examples

```csharp
// Called: int sh = cells.StandardHeightPixels;
public void Cells_Property_StandardHeightPixels()
{
    Workbook wb = LoadAsCsv("1,2,,,5,6\n\n\n1,2,,,5,6", new TxtLoadOptions());
    Assert.AreEqual(1, wb.Worksheets.Count, "Loaded sheet count");
    Cells cells = wb.Worksheets[0].Cells;
    for (int i = 0; i < 4; i++)
    {
        for (int j = 0; j < 8; j++)
        {
            if ((i == 0 || i == 3) && (j == 0 || j == 1 || j == 4 || j == 5))
            {
                Assert.AreEqual(j + 1, cells[i, j].IntValue);
            }
            else if (cells.CheckCell(i, j) != null)
            {
                Assert.Fail("Cell at column " + j + " should not be instantiated");
            }
        }
    }
    int sh = cells.StandardHeightPixels;
    foreach(Row r in cells.Rows)
    {
        Assert.AreEqual(sh, cells.GetRowHeightPixel(r.Index));
    }
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


