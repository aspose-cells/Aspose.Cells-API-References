---
title: Row.IsHeightMatched
second_title: Aspose.Cells for .NET API Reference
description: Row property. Indicates whether the row height matches current default font setting of the workbook. True of this property also denotes the row height is automatic without custom height value set by user
type: docs
url: /net/aspose.cells/row/isheightmatched/
---
## Row.IsHeightMatched property

Indicates whether the row height matches current default font setting of the workbook. True of this property also denotes the row height is "automatic" without custom height value set by user.

```csharp
public bool IsHeightMatched { get; set; }
```

### Remarks

When this property is true, if the content in this row changes, generally the row height needs to be re-calculated(such as by [`AutoFitRows`](../../worksheet/autofitrows/)) to get the same result with what is shown in ms excel when you opening the workbook in it.

### Examples

```csharp
// Called: Assert.IsFalse(workbook.Worksheets[0].Cells.Rows[5].IsHeightMatched);
[Test]
        public void Property_IsHeightMatched()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet52214.xlsx");
            foreach (Worksheet workSheet in workbook.Worksheets)
            {
                SetWorksheetAutoFitOptions_CellsNet52214(workSheet);
                //SetWorksheetPageSetupOptions(workSheet);
            }

            Assert.IsFalse(workbook.Worksheets[0].Cells.Rows[5].IsHeightMatched);
            workbook.Save(Constants.destPath + "CellsNet52214.xlsx", SaveFormat.Xlsx);
        }
```

### See Also

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


