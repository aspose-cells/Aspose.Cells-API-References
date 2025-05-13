---
title: Worksheet.IsGridlinesVisible
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets or sets a value indicating whether the gridlines are visible.Default is true
type: docs
url: /net/aspose.cells/worksheet/isgridlinesvisible/
---
## Worksheet.IsGridlinesVisible property

Gets or sets a value indicating whether the gridlines are visible.Default is true.

```csharp
public bool IsGridlinesVisible { get; set; }
```

### Examples

```csharp
// Called: wb.Worksheets[0].IsGridlinesVisible = true;
public void Worksheet_Property_IsGridlinesVisible()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA43180/";

    HtmlLoadOptions opts = new HtmlLoadOptions();
    opts.AutoFitColsAndRows = true;
    Workbook wb = new Workbook(filePath + "report.html", opts);
    wb.Worksheets[0].IsGridlinesVisible = true;

    Cell a3 = wb.Worksheets[0].Cells["A3"];
    Assert.AreEqual(a3.GetStyle().ForegroundColor, Color.FromArgb(255, 192, 192, 192));

    wb.Save(CreateFolder(filePath) + "out.xlsx");
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


