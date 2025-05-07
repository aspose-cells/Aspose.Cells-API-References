---
title: StyleFlag.NumberFormat
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. Number format setting will be applied
type: docs
url: /net/aspose.cells/styleflag/numberformat/
---
## StyleFlag.NumberFormat property

Number format setting will be applied.

```csharp
public bool NumberFormat { get; set; }
```

### Examples

```csharp
// Called: StyleFlag styleFlag = new StyleFlag() { NumberFormat = true };
[Test]
        public void Property_NumberFormat()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Aspose.Cells.Range range = sheet.Cells.CreateRange(0, 0, 1, 1);
            sheet.Cells[0, 0].Value = 1234.56;
            Style style = workbook.CreateStyle();
            style.Custom = "_-€ #,##0.00;[Red]_-€ -#,##0.00";
            StyleFlag styleFlag = new StyleFlag() { NumberFormat = true };
            range.ApplyStyle(style, styleFlag);

            workbook.Save(Constants.destPath + "/CellsNet43664.ods");
            workbook = new Workbook(Constants.destPath + "/CellsNet43664.ods");
            Assert.AreEqual(sheet.Cells[0, 0].GetStyle().Custom, "_-€ #,##0.00;[Red]_-€ -#,##0.00");
        }
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


