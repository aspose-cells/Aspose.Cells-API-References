---
title: Style.IsTextWrapped
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets or sets a value indicating whether the text within a cell is wrapped
type: docs
url: /net/aspose.cells/style/istextwrapped/
---
## Style.IsTextWrapped property

Gets or sets a value indicating whether the text within a cell is wrapped.

```csharp
public bool IsTextWrapped { get; set; }
```

### Examples

```csharp
// Called: style.IsTextWrapped = true;
public void Style_Property_IsTextWrapped()
{
    Workbook wb = new Workbook();
    Style defaultStyle = wb.DefaultStyle;
    defaultStyle.Font.Name = "Arial";
    defaultStyle.Font.Size = 8;
    wb.DefaultStyle = defaultStyle;
    Worksheet ws = wb.Worksheets["Sheet1"]; 
    Cells cells = ws.Cells; 
    Cell cell = cells[0, 0];
    cell.PutValue("Voor meer informatie, nga naar");
    Style style = cell.GetStyle();
    style.IsTextWrapped = true;
    cell.SetStyle(style);
    ws.AutoFitRow(0);
    wb.Save(Constants.destPath + "example.xls");

    Assert.AreEqual(cells.GetRowHeight(0), 33.75,0.01);
}
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


