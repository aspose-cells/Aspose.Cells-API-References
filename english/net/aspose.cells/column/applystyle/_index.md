---
title: Column.ApplyStyle
second_title: Aspose.Cells for .NET API Reference
description: Column method. Applies formats for a whole column
type: docs
url: /net/aspose.cells/column/applystyle/
---
## Column.ApplyStyle method

Applies formats for a whole column.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |

### Examples

```csharp
// Called: sheet.Cells.Columns[2].ApplyStyle(style, new StyleFlag() { WrapText = true });
public void Column_Method_ApplyStyle()
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

    workbook.Save(Constants.destPath + "example.xlsx");//It formats text properly with wrap text
    workbook.Save(Constants.destPath + "example.ods");//Wrap text does not work properly
}
```

### See Also

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


