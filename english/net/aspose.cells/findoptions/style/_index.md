---
title: FindOptions.Style
second_title: Aspose.Cells for .NET API Reference
description: FindOptions property. The format to search for
type: docs
url: /net/aspose.cells/findoptions/style/
---
## FindOptions.Style property

The format to search for.

```csharp
public Style Style { get; set; }
```

### Examples

```csharp
// Called: options.Style = style;
[Test]
        public void Property_Style()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CellsNet40679.xlsx");
            Worksheet ws = wb.Worksheets[0];
            Style style = wb.CreateStyle();
            style.Font.Color = System.Drawing.Color.Blue;
            FindOptions options = new FindOptions();
            options.Style = style;

            Cells cells = ws.Cells;
            Cell cell = cells.Find(null, null, options);
            Assert.AreEqual(cell.Name, "F2");
        }
```

### See Also

* class [Style](../../style/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


