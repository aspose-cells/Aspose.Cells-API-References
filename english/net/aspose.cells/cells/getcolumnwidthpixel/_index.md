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
// Called: Assert.AreEqual(30, cells.GetColumnWidthPixel(12));
[Test]
        public void Method_Int32_()
        {
            Workbook wb = new Workbook(Constants.HtmlPath + &quot;CELLSJAVA-43948.xls&quot;);
            string savePath = _destFilesPath + &quot;CELLSJAVA-43948.html&quot;;

            wb.Save(savePath);

            Workbook reloadWb = new Workbook(savePath);
            Cells cells = reloadWb.Worksheets[0].Cells;
            Assert.AreEqual(52, cells.GetColumnWidthPixel(0));
            Assert.AreEqual(48, cells.GetColumnWidthPixel(1));
            Assert.AreEqual(41, cells.GetColumnWidthPixel(2));
            Assert.AreEqual(30, cells.GetColumnWidthPixel(12));
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


