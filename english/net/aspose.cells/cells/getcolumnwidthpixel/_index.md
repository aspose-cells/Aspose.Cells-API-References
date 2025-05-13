---
title: Cells.GetColumnWidthPixel
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Gets the width of the specified column in normal view in units of pixel
type: docs
url: /net/aspose.cells/cells/getcolumnwidthpixel/
---
## GetColumnWidthPixel(int) {#getcolumnwidthpixel}

Gets the width of the specified column in normal view, in units of pixel.

```csharp
public int GetColumnWidthPixel(int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Column index |

### Return Value

Width of column in normal view.

### Examples

```csharp
// Called: int t = ws2.Cells.GetColumnWidthPixel(1);
public void Cells_Method_GetColumnWidthPixel()
{
    var workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    var ws = workbook.Worksheets[0];
    var ws2 = workbook.Worksheets[1];
    var fromRange = ws.Cells.CreateRange(0, 0, 10, 10);
    int t = ws2.Cells.GetColumnWidthPixel(1);
    var toRange = ws2.Cells.CreateRange(0, 0, 10, 10);
    toRange.Copy(fromRange, new PasteOptions() { PasteType = PasteType.Default });
    Assert.AreEqual(t, ws2.Cells.GetColumnWidthPixel(1));
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetColumnWidthPixel(int, bool) {#getcolumnwidthpixel_1}

Gets the width of the specified column in normal view, in units of pixel.

```csharp
[Obsolete("Use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int GetColumnWidthPixel(int column, bool original)
```

| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Column index |
| original | Boolean | Indicates whether returning original width even when the column is hidden |

### Return Value

Width of column in normal view.

### Remarks

NOTE: This method is now obsolete. Instead, please use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method. This method will be removed 12 months later since April 2024. Aspose apologizes for any inconvenience you may have experienced.

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


