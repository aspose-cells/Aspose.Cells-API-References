---
title: StyleFlag.WrapText
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. Wrap text setting will be applied
type: docs
url: /net/aspose.cells/styleflag/wraptext/
---
## StyleFlag.WrapText property

Wrap text setting will be applied.

```csharp
public bool WrapText { get; set; }
```

### Examples

```csharp
// Called: sheet.Cells.Columns[2].ApplyStyle(style, new StyleFlag() { WrapText = true });
[Test]
        public void Property_WrapText()
        {
            Workbook workbook = new Workbook(); // Creating a Workbook object

            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells[2, 2].Value = "Use";
            sheet.Cells[2, 2].Value += "\n with word wrap on to create a new line";

            sheet.Cells[3, 2].Value = "Use";
            sheet.Cells[3, 2].Value += "\n with word wrap on to create a new line";

            sheet.Cells[4, 2].Value = "Use";
            sheet.Cells[4, 2].Value += "\n with word wrap on to create a new line";

            Style style = workbook.CreateStyle();

            //Set Text Wrap property to true
            style.IsTextWrapped = true;

            //Set Cell's Style
            sheet.Cells.Columns[2].ApplyStyle(style, new StyleFlag() { WrapText = true });

            workbook.Save(Constants.destPath + "CELLSNET47781.xlsx");//It formats text properly with wrap text
            workbook.Save(Constants.destPath + "CELLSNET47781.ods");//Wrap text does not work properly
        }
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


