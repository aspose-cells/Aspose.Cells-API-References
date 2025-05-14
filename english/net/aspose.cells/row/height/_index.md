---
title: Row.Height
second_title: Aspose.Cells for .NET API Reference
description: Row property. Gets and sets the row height in unit of Points
type: docs
url: /net/aspose.cells/row/height/
---
## Row.Height property

Gets and sets the row height in unit of Points.

```csharp
public double Height { get; set; }
```

### Examples

```csharp
// Called: Assert.Greater(wb.Worksheets[0].Cells.Rows[0].Height, 0);
public void Row_Property_Height()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"NET44699And44700And44701/";

    string savePath = CreateFolder(filePath);
    HtmlLoadOptions options = new HtmlLoadOptions();
    options.SupportDivTag = true;
    Workbook wb = null;
    wb = new Workbook(filePath + "sample1.html", options);
    Assert.AreEqual(wb.Worksheets[0].Cells["A1"].StringValue, "This is a div with display set to none");
    Assert.Greater(wb.Worksheets[0].Cells.Rows[0].Height, 0);
    wb.Save(savePath + "out1.xlsx");

    wb = new Workbook(filePath + "sample2.html", options);
    Assert.AreEqual(wb.Worksheets[0].Cells["A1"].StringValue, "This is a div with display set to block");
    Assert.Greater(wb.Worksheets[0].Cells.Rows[0].Height, 0);
    wb.Save(savePath + "out2.xlsx");

    wb = new Workbook(filePath + "sample3.html", options);
    Assert.AreEqual(wb.Worksheets[0].Cells["A1"].StringValue, "This is just a plain div");
    Assert.Greater(wb.Worksheets[0].Cells.Rows[0].Height, 0);
    wb.Save(savePath + "out3.xlsx");

    wb = new Workbook(filePath + "pre.html", options);
    Assert.AreEqual(wb.Worksheets[0].Cells["A1"].StringValue, "This is hidden");
    Assert.Greater(wb.Worksheets[0].Cells.Rows[0].Height, 0);
    wb.Save(savePath + "pre.xlsx");
}
```

### See Also

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


