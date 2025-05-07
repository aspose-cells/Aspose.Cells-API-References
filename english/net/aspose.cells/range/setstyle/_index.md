---
title: Range.SetStyle
second_title: Aspose.Cells for .NET API Reference
description: Range method. Apply the cell style
type: docs
url: /net/aspose.cells/range/setstyle/
---
## SetStyle(Style, bool) {#setstyle_1}

Apply the cell style.

```csharp
public void SetStyle(Style style, bool explicitFlag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The cell style. |
| explicitFlag | Boolean | True, only overwriting formatting which is explicitly set. |

### Examples

```csharp
// Called: wb.Worksheets[0].Cells.CreateRange(0, 1, false).SetStyle(style, true);
[Test]
        public void Method_Boolean_()
        {
            Workbook wb = new Workbook();
            Style style = new CellsFactory().CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.Red;
            wb.Worksheets[0].Cells.CreateRange(0, 1, false).SetStyle(style, true);
           Assert.IsTrue( wb.Worksheets[0].Cells.Rows[0].GetCellOrNull(3) == null);
            wb.Save(Constants.destPath + "CELLSNET57109.xlsx");
        }
```

### See Also

* class [Style](../../style/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetStyle(Style) {#setstyle}

Sets the style of the range.

```csharp
public void SetStyle(Style style)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The Style object. |

### Examples

```csharp
// Called: range.SetStyle(style);
[Test]
        public void Method_Style_()
        {
            Workbook workbook = new Workbook();
            Worksheet ws = workbook.Worksheets[0];
            Cells cells = ws.Cells;

            Style style = workbook.CreateStyle();
            style.ForegroundColor = (Color.Yellow);
            style.Pattern = (BackgroundType.Solid);

            PasteOptions pstoption = new PasteOptions();
            pstoption.PasteType = (PasteType.Formats);
            pstoption.Transpose = (true);

            Aspose.Cells.Range range = cells.CreateRange(1, 1, 1, 4);
            range.SetStyle(style);

            Aspose.Cells.Range range2 = cells.CreateRange(6, 1, 9, 1);
            range2.Copy(range, pstoption);
            Assert.AreEqual(range2[0, 0].GetStyle().Pattern, BackgroundType.Solid);

       
        }
```

### See Also

* class [Style](../../style/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


