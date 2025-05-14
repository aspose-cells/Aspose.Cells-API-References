---
title: Title.Text
second_title: Aspose.Cells for .NET API Reference
description: Title property. Gets or sets the text of display unit label
type: docs
url: /net/aspose.cells.charts/title/text/
---
## Title.Text property

Gets or sets the text of display unit label.

```csharp
public override string Text { get; set; }
```

### Examples

```csharp
// Called: workbook.Worksheets[0].Charts[0].ValueAxis.Title.Text = "Alerts";
public void Title_Property_Text()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    workbook.Worksheets[0].Charts[0].ValueAxis.Title.Text = "Alerts";

    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


