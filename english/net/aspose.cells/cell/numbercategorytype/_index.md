---
title: Cell.NumberCategoryType
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Represents the category type of this cells number formatting
type: docs
url: /net/aspose.cells/cell/numbercategorytype/
---
## Cell.NumberCategoryType property

Represents the category type of this cell's number formatting.

```csharp
public NumberCategoryType NumberCategoryType { get; }
```

### Remarks

When cell's formatting pattern is combined with conditional formatting patterns, then the returned type is corresponding to the part which is used for current value of this cell. For example, if the formatting pattern for this cell is "#,##0;(#,##0);"-";@", then when cell's value is numeric and not 0, the returned type is Number; When cell's value is 0 or not numeric value, the returned type is Text.

### Examples

```csharp
// Called: Assert.AreEqual(NumberCategoryType.Date, cell.NumberCategoryType, "D2's NumberCategoryType");
[Test]
        public void Property_NumberCategoryType()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "Style/N43620_625404.xml");
            Cell cell = wb.Worksheets[0].Cells["D2"];
            Assert.AreEqual(CellValueType.IsDateTime, cell.Type, "D2's CellValueType");
            Assert.IsTrue(cell.GetStyle().IsDateTime, "D2's Style.IsDateTime");
            Assert.AreEqual(NumberCategoryType.Date, cell.NumberCategoryType, "D2's NumberCategoryType");
            cell = wb.Worksheets[0].Cells["D3"];
            Assert.AreEqual(CellValueType.IsDateTime, cell.Type, "D3's CellValueType");
            Assert.IsTrue(cell.GetStyle().IsDateTime, "D3's Style.IsDateTime");
            Assert.AreEqual(NumberCategoryType.Date, cell.NumberCategoryType, "D3's NumberCategoryType");
            Style style = cell.GetStyle();
            style.Custom = "yyyy-mm-dd;0.000";
            cell.SetStyle(style);
            Assert.AreEqual(CellValueType.IsDateTime, cell.Type, "CellValueType for CombinedFormatting with value " + cell.Value);
            Assert.IsTrue(cell.GetStyle().IsDateTime, "D3's Style.IsDateTime for CombinedFormatting with value " + cell.Value);
            Assert.AreEqual(NumberCategoryType.Date, cell.NumberCategoryType, "D2's NumberCategoryType");
            cell.PutValue(-3);
            Assert.AreEqual(CellValueType.IsNumeric, cell.Type, "CellValueType for CombinedFormatting with value " + cell.Value);
            Assert.IsTrue(cell.GetStyle().IsDateTime, "Style.IsDateTime for CombinedFormatting with value " + cell.Value);
            Assert.AreEqual(NumberCategoryType.Number, cell.NumberCategoryType, "D2's NumberCategoryType");
        }
```

### See Also

* enum [NumberCategoryType](../../numbercategorytype/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


