---
title: Font.IsBold
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets or sets a value indicating whether the font is bold
type: docs
url: /net/aspose.cells/font/isbold/
---
## Font.IsBold property

Gets or sets a value indicating whether the font is bold.

```csharp
public bool IsBold { get; set; }
```

### Examples

```csharp
// Called: Assert.IsFalse(fs.Font.IsBold);
[Test]
        public void Property_IsBold()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsJava44859_1.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["B3"];
            Style style = cell.GetStyle();
            style.Number = (0);//this will denote as "General"
                               //apply the style back to the cell.
            cell.SetStyle(style);
            string str = ("<html><p><strong>This is Strong 1</strong></p><p><strong>This is Strong 2</strong></p>This is not Strong text</html>");
            cell.HtmlString = str;
            int index = cell.StringValue.IndexOf("not");
            FontSetting fs = cell.Characters(index, 3);
            Assert.IsFalse(fs.Font.IsBold);
        }
```

### See Also

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


