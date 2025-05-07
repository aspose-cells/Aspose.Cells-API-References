---
title: Cells.StandardWidth
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets or sets the default column width in the worksheet in unit of characters
type: docs
url: /net/aspose.cells/cells/standardwidth/
---
## Cells.StandardWidth property

Gets or sets the default column width in the worksheet, in unit of characters.

```csharp
public double StandardWidth { get; set; }
```

### Examples

```csharp
// Called: cells.StandardWidth = 20.1;
[Test]
        public void Property_StandardWidth()
        {
            caseName = "testStandardWidth_Excel2007_001";
            Workbook workbook = new Workbook();

            Style style = workbook.DefaultStyle;
            Font font = style.Font;
            font.Size = 10;
            font.Name = "Arial";
            workbook.DefaultStyle = style;
            Cells cells = workbook.Worksheets[0].Cells;
            cells.StandardWidth = 20.1;

            checkStandardWidth_Excel2007_001(workbook);
            workbook.Save(Constants.destPath + " testStandardWidth.xlsx");
            workbook = new Workbook(Constants.destPath + " testStandardWidth.xlsx");
            checkStandardWidth_Excel2007_001(workbook);
            workbook.Save(Constants.destPath + " testStandardWidth.xml", SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + " testStandardWidth.xml");
            workbook.Save(Constants.destPath + " testStandardWidth.xls");
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


