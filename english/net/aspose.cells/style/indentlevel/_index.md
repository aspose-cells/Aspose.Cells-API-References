---
title: Style.IndentLevel
second_title: Aspose.Cells for .NET API Reference
description: Style property. Represents the indent level for the cell or range. Can only be an integer from 0 to 250
type: docs
url: /net/aspose.cells/style/indentlevel/
---
## Style.IndentLevel property

Represents the indent level for the cell or range. Can only be an integer from 0 to 250.

```csharp
public int IndentLevel { get; set; }
```

### Remarks

If text horizontal alignment type is set to value other than left or right, indent level will be reset to zero.

### Examples

```csharp
// Called: Assert.AreEqual(b7.GetStyle().IndentLevel, 2);
[Test]
        public void Property_IndentLevel()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;JAVA40251_&quot;;
            Workbook wb = new Workbook(filePath + &quot;ARTIF_exhibits.xlsx&quot;);
            PdfSaveOptions options = new PdfSaveOptions();
            options.OnePagePerSheet = true;
            Worksheet sheet = wb.Worksheets[&quot;GICS Sector Exposure&quot;];
            Cells cells = sheet.Cells;
            Cell b6 = cells[&quot;B6&quot;];
            Cell b7 = cells[&quot;B7&quot;];
            Assert.AreEqual(b6.GetStyle().HorizontalAlignment, TextAlignmentType.Center);
            Assert.AreEqual(b6.GetStyle().IndentLevel, 0);

            Assert.AreEqual(b7.GetStyle().HorizontalAlignment, TextAlignmentType.Right);
            Assert.AreEqual(b7.GetStyle().IndentLevel, 2);

            sheet.PivotTables[0].CalculateData();

            Assert.AreEqual(b6.GetStyle().HorizontalAlignment, TextAlignmentType.Center);
            Assert.AreEqual(b6.GetStyle().IndentLevel, 0);

            Assert.AreEqual(b7.GetStyle().HorizontalAlignment, TextAlignmentType.Right);
            Assert.AreEqual(b7.GetStyle().IndentLevel, 2);

            wb.Save(CreateFolder(filePath) + &quot;out.pdf&quot;, options);
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


