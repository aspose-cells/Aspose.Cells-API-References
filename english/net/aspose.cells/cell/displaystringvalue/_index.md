---
title: Cell.DisplayStringValue
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets the formatted string value of this cell by cells display style
type: docs
url: /net/aspose.cells/cell/displaystringvalue/
---
## Cell.DisplayStringValue property

Gets the formatted string value of this cell by cell's display style.

```csharp
public string DisplayStringValue { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual("a3f", cell.DisplayStringValue);
public void Cell_Property_DisplayStringValue()
{
    Workbook wb = new Workbook();
    Cell cell = wb.Worksheets[0].Cells[0, 0];
    Style style = cell.GetStyle();
    style.Custom = "# ##/##\\\"";
    cell.SetStyle(style);
    cell.PutValue(3);
    Assert.AreEqual("3\"", cell.DisplayStringValue);
    style.Custom = "\"a\"#\"b\" \"c\"##\"d\"/\"e\"##";
    cell.SetStyle(style);
    Assert.AreEqual("a3", cell.DisplayStringValue);
    style.Custom = "\"a\"#\"b\" \"c\"##\"d\"/\"e\"##\"f\"";
    cell.SetStyle(style);
    Assert.AreEqual("a3f", cell.DisplayStringValue);
    cell.PutValue(1.234);
    Assert.AreEqual("a1b c11d/e47f", cell.DisplayStringValue);
    style.Custom = "\"a\"#\"b\"\"c\"##\"d\"/\"e\"##\"f\"";
    cell.SetStyle(style);
    cell.PutValue(3);
    Assert.AreEqual("a3f", cell.DisplayStringValue);
    cell.PutValue(1.234);
    Assert.AreEqual("a1bc11d/e47f", cell.DisplayStringValue);
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


